**Bug ID:** BR_SRP_001

**Title:** Broken Images Are Displayed on Some Products in the Search Results Page

**Type:** Functional

**Priority:** Low

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Summary:**

 When a user searches for a specific author (eg "Kohei Horikoshi") on the Search Results Page, some product listings display broken images instead of the actual book cover art. The products are still listed with their titles and prices but the images fail to load, resulting in a degraded browsing experience.

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Click on the search bar
3. Type "Kohei Horikoshi" and press Enter or click the search icon
4. Observe the product images displayed on the Search Results Page
5. Navigate to the 7th page 

**Expected Result:**

 All products returned on the SRP should display their correct book cover images with no broken image icons or placeholder images visible

**Actual Result:** 

One or more product listings on the SRP display broken images instead of the correct book cover art, leaving empty or broken image placeholders visible alongside the product details

**Additional Information**

This issue is reproduceable in the filter section after applying multiple filters in the SRP

<img width="1284" height="590" alt="broken image booksa million" src="https://github.com/user-attachments/assets/7cc72e19-02df-46d6-82dc-c6d59717ea89" />


---

**Additional information:**

The Issue persists in searches with results exceeding 6 pages 

---

**Bug ID:** BR_SRP_002

**Title:** User Receives an Error Message When Searching for Books Using an ISBN Number

**Type:** Functional

**Priority:** Medium

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Summary:** 

When a user attempts to search for a book using a valid ISBN number, the Search Results Page fails to return the expected product and instead displays a "No Results Found" message. This prevents users from locating specific books via ISBN, which is a standard and expected search method on an e-commerce book platform. A workaround exists by searching for the book title or author name directly.

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Click on the search bar
3. Type the ISBN number "9780747532743" (Harry Potter and the Philosopher's Stone) and press Enter or click the search icon
4. Observe the Search Results Page

**Expected Result:**

 The SRP loads and displays the correct book matching the ISBN entered — in this case, Harry Potter and the Philosopher's Stone by J.K. Rowling — along with its title, cover image, format options, and price

**Actual Result:** 

The SRP displays a "No Results Found" message despite the ISBN being valid and the book being available on the platform

**Workaround:** 

The user can search for the book using its title or author name instead of the ISBN number to locate the product successfully

<img width="1892" height="964" alt="search query" src="https://github.com/user-attachments/assets/30ee3ea7-5f7e-4189-9520-225c4815757d" />

---

**Bug ID:** BR_CART_001

**Title:** User Cannot Proceed to Checkout and Is Redirected to an Error Page

**Type:** Functional

**Priority:** Critical

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Summary:** 

When a user attempts to proceed to checkout after adding items to the cart, they are blocked from accessing the checkout page and are instead redirected to an error page stating "Sorry, you have been blocked. You are unable to access booksamillion.com." This completely prevents the user from completing a purchase and represents a critical break in the core user flow.

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for any book and navigate to its Product Description Page
3. Add the item to the cart
4. Click on the cart icon in the header
5. On the cart page, click the Checkout button
6. Observe the page behaviour

**Expected Result:**

 The user is redirected to the checkout page where they can review their order, enter their delivery details, and proceed with payment successfully

**Actual Result:** 

The user is blocked from proceeding to checkout and is redirected to an error page displaying the following message: "Sorry, you have been blocked. You are unable to access booksamillion.com." The user is completely unable to complete their purchase.

<img width="1899" height="910" alt="image" src="https://github.com/user-attachments/assets/20a5a044-aed3-4cc2-b7b5-3ef48c3330ff" />

---

**Bug ID:** BR_UX_001

**Title:** Site Repeatedly Triggers CAPTCHA/Robot Verification Check During Normal User Interaction

**Type:** UX / Functional

**Priority:** Medium

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Summary:** 

After interacting with the Books-A-Million website for approximately 5 to 10 minutes, the site intermittently triggers a CAPTCHA or human verification check when the user clicks on a button or navigates between pages. This interrupts the normal browsing and purchasing flow and creates a frustrating experience for legitimate users. The check appears to occur repeatedly throughout the session rather than as a one-time verification.

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Interact with the site normally — browse the homepage, search for books, click on products, and add items to the cart
3. Continue interacting with the site for approximately 5 to 10 minutes
4. Click on any button or navigate to a new page
5. Observe whether a CAPTCHA or human verification prompt appears
6. Complete the verification check and continue interacting with the site
7. Observe whether the verification check reappears after further interaction

**Expected Result:** 

A legitimate user should only be prompted to complete a human verification check once per session if at all. Normal browsing, searching, and purchasing interactions should not repeatedly trigger verification prompts throughout the session

**Actual Result:** 

The site intermittently triggers a CAPTCHA or human verification check every 5 to 10 minutes of normal user interaction, repeatedly interrupting the browsing and purchasing flow for legitimate users

**Additional Information:** 

This issue is likely related to the platform's bot detection or security configuration being overly aggressive, incorrectly flagging normal user behaviour as suspicious activity. This is consistent with the block error observed in BR_CART_001 during checkout, suggesting both issues may share the same root cause in the platform's security layer. It is recommended that the security configuration be reviewed to better distinguish between legitimate user activity and actual bot behaviour


<img width="1897" height="1025" alt="Screenshot 2026-06-12 105552" src="https://github.com/user-attachments/assets/8e0018b1-3ec8-4387-8b7a-5fc90f239ae9" />

---

**Bug ID:** BR_CART_002

**Title:** Using the Browser Back Button After Removing an Item Restores the Removed Item

**Type:** Functional

**Priority:** Medium

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Summary:** When a user removes an item from the cart and then clicks the browser back button, the previously removed item reappears in the cart. This means the cart does not correctly reflect the user's intended actions and may lead to the user unknowingly purchasing an item they had already removed.

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for any book and add it to the cart
3. Add a second book to the cart
4. Navigate to the cart
5. Remove one item from the cart using the remove button
6. Confirm the item has been successfully removed from the cart
7. Click the browser back button
8. Observe the cart contents

**Expected Result:** The removed item remains deleted from the cart and does not reappear after using the browser back button. The cart count and subtotal should continue to reflect the correct state after the item was removed

**Actual Result:** The previously removed item reappears in the cart after the user clicks the browser back button, restoring the cart to its previous state before the item was removed


<img width="1905" height="1003" alt="image" src="https://github.com/user-attachments/assets/4077bbca-6318-4053-8aa7-4c36d7fee386" />


<img width="1905" height="1003" alt="image" src="https://github.com/user-attachments/assets/fde8c46e-c321-4ac8-af42-67cacea28625" />
