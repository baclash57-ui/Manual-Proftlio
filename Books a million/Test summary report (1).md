## Report Details

| Field | Details |
| --- | --- |
| Project | Books-A-Million – booksamillion.com |
| Prepared By | Obinna Japhet Prosper |
| Test Date | February 18, 2026 |
| Environment | Windows 11 |
| Browser | Microsoft Edge (Latest Stable) |
| Test Cycle | Cycle 1 – Functional & UX Testing |
| Report Status | Final |

---

## Objective

The objective of this test cycle was to validate the core functionalities and user experience of the Books-A-Million e-commerce website (booksamillion.com). Testing focused on ensuring that users can successfully browse, search for, select, and purchase books with accurate system behaviour, proper navigation, and consistent pricing. Testing was conducted manually on a Windows 11 desktop machine using Microsoft Edge and covered the end-to-end user journey from the homepage through to the checkout entry point.

---

## Scope Summary

| Area | In Scope | Out of Scope |
| --- | --- | --- |
| Homepage | ✅ |  |
| Search & Filter | ✅ |  |
| Product Description Page (PDP) | ✅ |  |
| Cart | ✅ |  |
| User Experience & Flow | ✅ |  |
| Book Reviews & Review Search |  | ✅ |
| Social Media Links & Integrations |  | ✅ |
| Footer – External Company Info & Help Pages |  | ✅ |
| Toys & Games Section |  | ✅ |
| Millionaire's Club Features |  | ✅ |
| Mobile & Tablet Responsiveness |  | ✅ |
| Cross-Browser Compatibility Testing |  | ✅ |
| Performance & Load Testing |  | ✅ |
| Accessibility (WCAG) Testing |  | ✅ |

---

## Test Execution Summary

| Area | Total Test Cases | Passed | Failed | Blocked | Not Executed |
| --- | --- | --- | --- | --- | --- |
| Homepage | 7 | 7 | 0 | 0 | 0 |
| Search & Filter | 6 | 5 | 1 | 0 | 0 |
| Product Description Page | 6 | 6 | 0 | 0 | 0 |
| Cart | 7 | 6 | 1 | 0 | 0 |
| User Experience & Flow | 5 | 3 | 2 | 0 | 0 |
| **Total** | **31** | **27** | 4 | **0** | **0** |

---

## Test Pass Rate

| Metric | Result |
| --- | --- |
| Total Test Cases Executed | 31 |
| Total Passed | 27 |
| Total Failed | 4 |
| Overall Pass Rate | 87.10% |
| Exit Criteria Threshold | 90% |
| Exit Criteria Met | ❌ Not Met |

> Note: The overall pass rate of 87.10% falls slightly below the 90% exit criteria threshold defined in the test plan. This is primarily driven by BR_CART_001 which completely blocks the checkout flow, and BR_UX_001 which repeatedly interrupts normal user interaction site-wide. Immediate resolution of all High and Medium priority defects is strongly recommended before any further action is taken.
> 

---

## Defects Summary

| Bug ID | Title | Area | Priority | Status |
| --- | --- | --- | --- | --- |
| BR_SRP_001 | Broken images displayed on some products in the SRP | Search Results Page | Low | Open |
| BR_SRP_002 | User receives error message when searching by ISBN | Search Results Page | Medium | Open |
| BR_CART_001 | User cannot proceed to checkout and is redirected to an error page | Cart – Checkout Flow | High | Open |
| BR_CART_002 | Browser back button after removing an item restores the removed item | Cart | Medium | Open |
| BR_UX_001 | Site repeatedly triggers CAPTCHA verification during normal user interaction | Site-wide | Medium | Open |

---

## Defects by Priority

| Priority | Count |
| --- | --- |
| High | 1 |
| Medium | 3 |
| Low | 1 |
| **Total** | **5** |

---

## Test Results by Area

**Homepage**
A total of 7 test cases were executed for the homepage and all were passed. Navigation menus, promotional banners, category links, the company logo redirect, product carousels, and the Best Sellers section all functioned as expected. The major failure was related to BR_UX_001 being triggered during homepage interaction

**Search & Filter**
A total of 6 test cases were executed for the Search and Filter section. 5 passed and 1 failed. Searching by title and author name returned correct results and filter functionality including single filter selection and clearing all filters performed as expected. The  failure is linked to BR_SRP_001 where broken images appeared on the SRP for author-based searches, and BR_SRP_002 which was found during exploratory testing where a valid ISBN search returned a No Results Found message instead of the expected product.

**Product Description Page (PDP)**
A total of 6 test cases were executed for the PDP.  All 6 passed . Product title accuracy, format switching, price updates, stock status, author redirect, product description expand and collapse, and the Add to Cart button all functioned correctly. 

**Cart**
A total of 7 test cases were executed for the Cart section. 6 passed and 1 failed. Adding items to the cart, updating quantities, removing items, verifying subtotal calculations, and cart persistence across page navigation all functioned correctly. One failures was linked to BR_CART_002 where using the browser back button after removing an item incorrectly restores the removed item to the cart the other  BR_CART_001 where the user is completely blocked from proceeding to checkout and redirected to an error page is gotten from an exploratory test.

**User Experience & Flow**
A total of 5 test cases were executed for the User Experience and Flow section. 3 passed and 2 failed. The search bar visibility across all in-scope pages and cart icon count consistency both performed as expected. The 3 failures were linked to BR_CART_001 blocking the full end-to-end flow at the checkout step, BR_UX_001 where the CAPTCHA check repeatedly interrupted the user mid-session, and the site displaying a blocked error page during a legitimate checkout interaction.

---

## Risk Assessment

**BR_CART_001** poses the highest risk to the platform. A user being completely blocked from checkout means no transactions can be completed, which has a direct and immediate impact on revenue. This should be treated as the top priority defect for resolution.

**BR_UX_001** carries a Medium-High risk level despite its Medium priority rating. The repeated CAPTCHA interruptions affect all users throughout their entire session and significantly increase the likelihood of session abandonment at any stage of the user journey. Combined with BR_CART_001, both bugs appear to share the same root cause in the platform's bot detection and security configuration and should be investigated and resolved together.

**BR_CART_002** presents a medium risk to purchase accuracy. A user who unknowingly proceeds to checkout with an item they had already removed may lose trust in the platform upon noticing the discrepancy, leading to cart abandonment or a negative post-purchase experience.

**BR_SRP_002** carries medium risk as it removes a key search method for users who rely on ISBN to locate specific book editions. A workaround exists but the absence of this functionality falls below the expected standard for a book e-commerce platform.

**BR_SRP_001** carries low risk as product information remains accessible despite the broken images. It should however be resolved to maintain a professional and trustworthy browsing experience.

---

## Entry & Exit Criteria Status

| Criteria | Status |
| --- | --- |
| 100% of test cases executed | ✅ Met |
| No P1 blocking defects identified | ❌ Not Met (BR_CART_001 is a full checkout blocker) |
| All High severity defects documented | ✅ Met |
| 90% minimum pass rate achieved | ❌ Not Met (87.10% achieved) |
| Core user flows function without blocking issues | ❌ Not Met (Checkout flow is completely blocked) |
| Test summary report produced | ✅ Met |
| Stakeholder sign-off obtained | ⏳ Pending |

---

## Recommendations

- Immediately investigate and resolve BR_CART_001 as it is a complete blocker on the checkout flow with direct revenue impact
- Review and recalibrate the platform's bot detection and security configuration to resolve both BR_CART_001 and BR_UX_001 simultaneously as they likely share the same root cause
- Fix the cart state management to ensure removed items do not reappear when the browser back button is used (BR_CART_002)
- Fix the ISBN search logic to ensure valid ISBN numbers return the correct product results (BR_SRP_002)
- Resolve the broken image issue on the SRP for author-based searches (BR_SRP_001)
- Conduct a full regression test across all in-scope areas after all High and Medium priority defects have been resolved
- Consider expanding test coverage in the next cycle to include mobile and tablet responsiveness and cross-browser compatibility

---

## Overall Verdict

> ⚠️ CRITICAL DEFECTS IDENTIFIED – IMMEDIATE ACTION REQUIRED
The test cycle has been completed however critical defects have been identified that are actively impacting live users. BR_CART_001 completely blocks the checkout flow preventing users from completing purchases, and BR_UX_001 is repeatedly interrupting normal browsing sessions site-wide. The overall pass rate of 87.10% falls slightly below the required 90% threshold. Immediate investigation and resolution of all High and Medium priority defects is strongly recommended to prevent further impact on user experience and revenue.
> 

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
