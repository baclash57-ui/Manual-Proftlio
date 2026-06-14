## Report Details

| Field | Details |
| --- | --- |
| Project | Books-A-Million – booksamillion.com |
| Prepared By | Obinna Japhet Prosper |
| Test Date | February 18, 2026 |
| Environment | Windows 11 |
| Browser | Microsoft Edge (Latest Stable) |
| Total Bugs Reported | 6 |
| Report Status | Final |

---

## Bug Count by Prioritya

| Priority | Count |
| --- | --- |
| High | 1 |
| Medium | 4 |
| Low | 1 |
| **Total** | **6** |

---

## Bug Count by Type

| Type | Count |
| --- | --- |
| Functional | 5 |
| UX / Functional | 1 |
| **Total** | **6** |

---

## Bug Summary Table

| Bug ID | Title | Type | Priority | Reproducibility | Status |
| --- | --- | --- | --- | --- | --- |
| BR_SRP_001 | Broken images displayed on some products in the SRP | Functional | Low | Always | Open |
| BR_SRP_002 | User receives error message when searching for books using ISBN | Functional | Medium | Always | Open |
| BR_CART_001 | User cannot proceed to checkout and is redirected to an error page | Functional | High | Always | Open |
| BR_CART_002 | Using the browser back button after removing an item restores the removed item | Functional | Medium | Always | Open |
| BR_UX_001 | Site repeatedly triggers CAPTCHA verification during normal user interaction | UX / Functional | Medium | Always | Open |

---

## Bug Descriptions

---

**BR_SRP_001 – Broken Images Are Displayed on Some Products in the Search Results Page**

- **Type:** Functional
- **Priority:** Low
- **Status:** Open
- **Area Affected:** Search Results Page (SRP)
- **Description:** When a user searches for a specific author (e.g., "Kohei Horikoshi"), some product listings on the SRP display broken images instead of the correct book cover art. The products are still listed with their titles and prices but the images fail to load correctly.
- **Workaround:** None required as the product details are still accessible despite the broken images.
- **Impact:** Low impact on core functionality. However it creates a visually degraded browsing experience and may reduce user confidence in the platform, particularly for users browsing by visual recognition of book covers.

---

**BR_SRP_002 – User Receives an Error Message When Searching for Books Using an ISBN Number**

- **Type:** Functional
- **Priority:** Medium
- **Status:** Open
- **Area Affected:** Search – Search Results Page (SRP)
- **Description:** When a user searches for a book using a valid ISBN number (e.g., 9780747532743 – Harry Potter and the Philosopher's Stone), the SRP returns a "No Results Found" message despite the book being available on the platform. ISBN search is a standard and expected functionality on an e-commerce book platform.
- **Workaround:** The user can search for the book using its title or author name instead of the ISBN number.
- **Impact:** Medium impact. While a workaround exists, the inability to search by ISBN removes a key search method that users — particularly librarians, educators, and avid readers — rely on to find specific editions of books. This directly affects the search functionality user flow.

---

**BR_CART_001 – User Cannot Proceed to Checkout and Is Redirected to an Error Page**

- **Type:** Functional
- **Priority:** High
- **Status:** Open
- **Area Affected:** Cart – Checkout Flow
- **Description:** When a user attempts to proceed to checkout after adding items to the cart, they are redirected to an error page displaying the message "Sorry, you have been blocked. You are unable to access booksamillion.com." The user is completely unable to complete a purchase. This is likely caused by the platform's security or bot detection system incorrectly flagging legitimate user activity during the checkout process.
- **Workaround:** None identified. The user cannot complete a purchase under any circumstances while this bug is active.
- **Impact:** This is the most critical bug identified in this test cycle. It represents a complete blocker on the core purchase flow, preventing any user from completing a transaction on the platform. This directly impacts revenue and should be treated as an urgent priority for investigation and resolution.

---

**BR_CART_002 – Using the Browser Back Button After Removing an Item Restores the Removed Item**

- **Type:** Functional
- **Priority:** Medium
- **Status:** Open
- **Area Affected:** Cart
- **Description:** When a user removes an item from the cart and subsequently clicks the browser back button, the previously removed item reappears in the cart, restoring it to its previous state. This means the cart does not correctly reflect the user's intended actions after using browser navigation.
- **Workaround:** The user should avoid using the browser back button after removing items and instead use the site's own navigation links to move between pages.
- **Impact:** This bug poses a risk to purchase accuracy. A user who removes an item with the intention of not purchasing it may unknowingly proceed to checkout with the item still in their cart if they use the browser back button. This is likely caused by the browser caching the previous cart state rather than fetching the updated cart from the server.

---

**BR_UX_001 – Site Repeatedly Triggers CAPTCHA/Robot Verification Check During Normal User Interaction**

- **Type:** UX / Functional
- **Priority:** Medium
- **Status:** Open
- **Area Affected:** Site-wide
- **Description:** After approximately 5 to 10 minutes of normal interaction with the site, the platform intermittently triggers a CAPTCHA or human verification check when the user clicks a button or navigates between pages. The check reappears repeatedly throughout the session rather than as a one-time verification, continuously interrupting the browsing and purchasing flow for legitimate users.
- **Workaround:** The user must complete the CAPTCHA verification check each time it appears in order to continue interacting with the site. There is no way to prevent the check from reappearing during the session.
- **Impact:** This bug creates a significantly degraded user experience for all legitimate users. The repeated interruption of normal browsing and purchasing activity is likely to increase session abandonment, particularly during critical moments such as searching for a product or proceeding to checkout. Combined with BR_CART_001, this suggests the platform's bot detection system is overly aggressive and may be impacting a large portion of genuine users across the site.

---

## Notable Observations

- BR_CART_001 and BR_UX_001 are both likely caused by the same root cause — an overly aggressive bot detection and security configuration — and should be investigated and resolved together
- BR_CART_002 is a cart state management issue that poses a direct risk to purchase accuracy and should be addressed alongside BR_CART_001 as part of a focused cart regression fix
- Two bugs (BR_SRP_001 and BR_SRP_002) are isolated to the Search Results Page, suggesting the SRP may benefit from a broader focused investigation beyond these specific scenarios
- All 5 bugs are consistently reproducible at 100% (Always), indicating systemic issues rather than intermittent edge cases

---

## Risk Assessment

**BR_CART_001** poses the highest risk to the platform. A user being completely blocked from checkout means zero transactions can be completed, which has a direct and immediate impact on revenue. This should be treated as the top priority defect for resolution.

**BR_UX_001** carries a Medium-High risk level despite its Medium priority rating. The repeated CAPTCHA verification checks affect all users throughout their entire session and significantly increase the likelihood of session abandonment. Combined with BR_CART_001, both bugs appear to share the same root cause and should be investigated and resolved together as a matter of urgency.

**BR_CART_002** carries medium risk due to its potential impact on purchase accuracy. A user who unknowingly proceeds to checkout with an item they had previously removed may lose trust in the platform upon noticing the discrepancy, leading to cart abandonment or a negative post-purchase experience.

**BR_SRP_002** carries medium risk as it removes the ability to search by ISBN, a key search method for users seeking specific book editions. A workaround exists but the absence of ISBN functionality falls below the expected standard for a book e-commerce platform.

**BR_SRP_001** carries low risk as product information remains accessible despite the broken images. However it should be resolved to maintain a professional and trustworthy browsing experience.

---

## Recommendations

- **Immediately investigate and resolve BR_CART_001** as it is a complete blocker on the checkout flow with direct revenue impact
- Review and recalibrate the platform's bot detection and security configuration to resolve both BR_CART_001 and BR_UX_001 simultaneously as they likely share the same root cause
- Fix the cart state management to ensure removed items do not reappear when the browser back button is used **(BR_CART_002)**
- Fix the ISBN search logic to ensure valid ISBN numbers return the correct product results **(BR_SRP_002)**
- Resolve the broken image issue on the SRP for author-based searches **(BR_SRP_001)**
- Conduct a full regression test across all in-scope areas after the above fixes have been applied

---

### Important Note:

This is a public website that was tested for personal purposes the bugs reported here might not be reproducible when tested again


## Sign-Off

| Field | Details |
| --- | --- |
| Prepared By | Obinna Japhet Prosper |
| Reviewed By |  |
| Approved By |  |
| Date | February 18, 2026 |
| Report Version | 1.0 |

---

