# Books-A-Million – Test Cases

---

## 1. User Experience & Flow

**TC_UF_OO1**

**Title:**

 User Undergoes Security verification before proceeding to homepage

**Summary:** 

Verify that the User is prompted to first verify he/she is human before they can proceed to the homepage of the website

**Priority**: High

**Status:** Passed

**Environment:** Windows 11

**Browser**: Microsoft Edge

**Status:** Passed

**Preconditions:**   The user is accessing the site for the first time or after a very long time (50 minutes)

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/ 
2. Click on the “verify that you are human” check box

**Expected Result:** 

The user is prompted to complete a one-time human verification check upon first access and is then allowed to proceed to the homepage without further interruption

**Actual Result:**

After clicking on the Link, the user is prompted to complete a one time human verification

After clicking the check box, the User is redirected to the homepage of the site

---

**TC_UX_001**

**Title:** Human verification check is triggered only once per session

**Summary:** Verify that the human verification or CAPTCHA check is triggered only once per user session and does not repeatedly interrupt normal browsing activity

**Priority:** High

**Status:** Failed 

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Complete the initial human verification check if prompted
3. Interact with the site normally for 5 to 10 minutes — browse the homepage, search for books, navigate to PDPs, and add items to the cart
4. Observe whether the verification check reappears during normal interaction

**Expected Result:** 

The human verification check appears only once at the start of the session and does not reappear during normal browsing and purchasing activity

**Actual Result:**

The human verification check appears several times when the user is interacting with the site

The human verification check appears whenever the user interacts with the site for over 5-10 minutes

---

**TC_UX_002**

**Title**: User can complete the full browsing to checkout flow without interruption

**Summary:** 

Verify that a user can complete the full end-to-end flow from homepage browsing through to the checkout entry point without being blocked or interrupted

**Priority:** High

**Status**: Failed

**Environment:** Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Browse the homepage and click on a book
3. View the product details on the PDP
4. Click Add to Cart
5. Navigate to the cart
6. Click the Proceed to Checkout button
7. Observe the page behaviour at each step

**Expected Result:** 

The user is able to complete each step of the flow without being blocked, redirected to an error page, or interrupted by repeated verification checks

**Actual Result:**

The user is unable to proceed to checkout page 

The human verification check appears several times when the user is interacting with the site

The human verification check appears whenever the user interacts with the site for over 5-10 minutes

---

**TC_UX_003**

**Title:** Navigation between pages is smooth and does not result in a blank screen

**Summary:**

 ****Verify that navigating between pages on the site does not result in a blank white screen or unresponsive state under normal network conditions

**Priority:** Medium

**Status**: Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Click on multiple navigation links including category pages, PDPs, and the cart
3. Observe the page load behaviour between each navigation

**Expected Result:**

 Each page loads correctly without displaying a blank white screen, unresponsive state, or error message during normal navigation

**Actual Result:**

 Each page loads correctly without displaying a blank white screen, unresponsive state, or error message during normal navigation

---

**TC_UX_004**

**Title:** Search bar is accessible and visible from all in-scope pages

**Summary:** 

Verify that the search bar is consistently visible and accessible from all in-scope pages including the homepage, SRP, PDP, and cart

**Priority:** Medium

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Observe the search bar on the homepage
3. Search for a book
4. Navigate to the SRP and PDP
5. Observe the search bar visibility and accessibility on each page

**Expected Result:** 

The search bar is consistently visible and functional in the header across all in-scope pages

**Actual Result:**

The search bar is consistently visible and functional in the header across all in-scope pages

---

**TC_UX_005 – NEGATIVE**

**Title:** Site does not display a blocked error page during normal checkout interaction

**Summary:**

 ****Verify that a legitimate user is not blocked or redirected to an error page when attempting to proceed to checkout

**Priority:** High

**Status: F**ailed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for any book and navigate to its PDP
3. Click Add to Cart
4. Navigate to the cart
5. Click the Proceed to Checkout button
6. Observe the page behaviour

**Expected Result:** 

The user is redirected to the checkout page where they can enter their delivery details and proceed with payment without being blocked or shown an error page

**Actual Result:**

The user is blocked from proceeding to the checkout page 

---

## 2. Homepage

---

**TC_HP_001**

**Title:** Homepage loads successfully 

**Summary:** 

Verify that the homepage loads completely with all elements visible and functional when navigated to on Users Browser Windows 11)

**Priority**: High

**Environment:** Windows 11

**Browser**: Microsoft Edge

**Status:** Passed

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Observe the page load
3. Check all visible elements including the header, navigation, banners, product sections, and footer

**Expected Result:** 

The homepage loads fully with all images, banners, navigation menus, and product sections visible with no broken elements or error messages

**Actual Result:**

The homepage loads fully with all images, banners, navigation menus, and product sections visible with no broken elements or error messages

---

**TC_HP_002**

**Title:** Company logo redirects user back to the homepage from any sub-page

**Summary:** 

Verify that clicking the BAM! company logo from any sub-page returns the user to the homepage

**Priority:** High

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Navigate to any sub-page (e.g., a category page or PDP)
3. Click the BAM! company logo in the header
4. Observe the page behaviour

**Expected Result:** 

The user is redirected back to the homepage regardless of which page they were on

**Actual Result:**

The user is redirected back to the homepage regardless of which page they were on

---

**TC_HP_003**

**Title:** Main promotional banners redirect to the correct campaign pages

**Summary:** Verify that clicking the main promotional banners on the homepage redirects the user to the correct corresponding campaign or offer page

**Priority:** Medium

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Locate the main promotional banners on the homepage (e.g., 40% off February Releases, 20% off All Manga)
3. Note the expected destination indicated by the banner
4. Click on the banner
5. Observe the page the user is redirected to

**Expected Result:** 

The user is redirected to the correct campaign or offer page that matches the content of the banner clicked

**Actual Result:**

The user is redirected to the correct campaign or offer page that matches the content of the banner clicked

---

**TC_HP_004**

**Title:** Category navigation links redirect to the correct filtered product gallery

**Summary:** 

Verify that clicking category-specific navigation links (e.g., Manga, Kids) leads the user to the correct filtered product gallery

**Priority:** High

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Locate the category navigation links in the header or navigation menu
3. Click on a category link (e.g., Manga)
4. Observe the page that loads

**Expected Result:** 

The user is redirected to the correct product gallery filtered to show only items belonging to the selected category

**Actual Result:**

The user is redirected to the correct product gallery filtered to show only items belonging to the selected category

---

**TC_HP_005**

**Title:** All images on the homepage load correctly without broken placeholders

**Summary:** 

Verify that all images including book covers, promotional banners, and section images load correctly on the homepage

**Priority:** Medium

**Status:** Passed

**Environment**: Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Scroll through the entire homepage from top to bottom
3. Observe all images including banners, book covers, and promotional section images

**Expected Result:** 

All images load correctly with no broken image icons, blank spaces, or placeholder images visible anywhere on the homepage

**Actual Result:**

All images load correctly with no broken image icons, blank spaces, or placeholder images visible anywhere on the homepage

---

**TC_HP_006**

**Title:** Trending Now / Today's Top Sellers carousel scrolls correctly

**Summary:**

 ****Verify that the Trending Now / Today's Top Sellers carousel on the homepage scrolls correctly and displays the correct books

**Priority:** Medium

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Scroll down to the Trending Now / Today's Top Sellers section
3. Click the left and right carousel arrows to scroll through the books
4. Observe the carousel behaviour

**Expected Result:** 

The carousel scrolls smoothly in both directions, displaying the correct book covers, titles, and prices with no broken images or layout issues

**Actual Result:**

The carousel scrolls smoothly in both directions, displaying the correct book covers, titles, and prices with no broken images or layout issues

---

**TC_HP_007 – NEGATIVE**

**Title:** Manual URL manipulation to an invalid category does not crash the site

**Summary:** Verify that navigating to an invalid or non-existent category URL does not crash the site and displays an appropriate error message

**Priority:** Low

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. In the browser address bar manually edit the URL to include an invalid category (e.g., https://www.booksamillion.com/invalidcategory123)
3. Press Enter and observe the page behaviour

**Expected Result:** 

The site does not crash and instead displays a user-friendly error message such as a 404 Page Not Found page with navigation options to return to the homepage

**Actual Result:**

The site does not crash and instead displays an error message saying: Sorry, we could not find the requested product

---

## 3. Search & Filter

---

**TC_SF_001**

**Title:** Searching by exact book title returns the correct book as the first result

**Summary:** 

Verify that entering an exact book title into the search bar returns the specific book as the first result on the SRP

**Priority:** High

**Status**: Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Click on the search bar in the header
3. Type an exact book title (e.g., "Harry Potter and the Philosopher's Stone")
4. Press Enter or click the search icon
5. Observe the first result on the SRP

**Expected Result:** 

The specific book matching the exact title entered appears as the first result on the SRP with the correct cover image, title, author, and price displayed

**Actual Result:**

The specific book matching the exact title entered appears as the first result on the SRP with the correct cover image, title, author, and price displayed

---

**TC_SF_002**

**Title:** Searching by author name returns all books written by that author

**Summary:** 

Verify that entering an author's name into the search bar returns all books written by that author on the SRP

**Priority:** High

**Status:** Passed 

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Click on the search bar
3. Type an author's name (e.g., "Kohei Horikoshi")
4. Press Enter or click the search icon
5. Observe the results on the SRP

**Expected Result**: 

The SRP displays all available books written by the searched author with correct cover images, titles, and prices

**Actual Result:**

The SRP displays all available books written by the searched author with correct cover images, titles, and prices

---

**TC_SF_003**

**Title:** Searching by a valid ISBN returns the exact matching product

**Summary:**

 ****Verify that entering a valid 13-digit ISBN into the search bar returns the exact matching book on the SRP

**Priority:** High

**Status:** Failed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Click on the search bar
3. Type a valid 13-digit ISBN (e.g., "9780747532743" – Harry Potter and the Philosopher's Stone)
4. Press Enter or click the search icon
5. Observe the results on the SRP

**Expected Result:** 

The SRP displays the exact book matching the ISBN entered with the correct title, author, cover image, and price

**Actual Result:**

The SRP displays a "No Results Found" message despite the ISBN being valid and the book being available on the platform

---

**TC_SF_004**

**Title:** Applying a single filter updates the product grid correctly

**Summary:** 

Verify that selecting one filter option on the SRP updates the product listing to show only items matching that filter

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for any book or author to land on the SRP
3. Locate the filter options panel
4. Select one filter option (e.g., Format: Hardcover)
5. Observe the product grid

**Expected Result:**

 The product grid updates to display only items that match the selected filter with no items from other formats shown

**Actual Result:**

 The product grid updates to display only items that match the selected filter with no items from other formats shown

---

**TC_SF_005 – NEGATIVE**

**Title:** Searching with only special characters displays a No Results Found message

**Summary:** 

Verify that entering only special characters into the search bar returns a user-friendly No Results Found message without crashing the page

**Priority:** Medium

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Click on the search bar
3. Type only special characters (e.g., "!@#$%")
4. Press Enter or click the search icon
5. Observe the SRP behaviour

**Expected Result:** 

The SRP displays a clear and user-friendly No Results Found message with no page crash or error and provides suggestions to help the user refine their search

**Actual Result:**

The SRP displays a clear and user-friendly No Results Found message with no page crash or error and provides suggestions to help the user refine their search

---

**TC_SF_006– NEGATIVE**

**Title:** Searching for a non-existent ISBN displays a helpful error message

**Summary:** Verify that entering an invalid or non-existent ISBN into the search bar displays a helpful error message rather than crashing the page

**Priority:** Medium

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Click on the search bar
3. Type a non-existent ISBN (e.g., "9999999999999")
4. Press Enter or click the search icon
5. Observe the SRP behaviour

**Expected Result:**

 ****The SRP displays a clear and helpful message informing the user that no product matching the ISBN was found 

**Actual Result:**

The page handles the task gracefully

 ****The SRP displays a clear and helpful message informing the user that no product matching the ISBN was found 

---

## 4. Product Description Page (PDP)

---

**TC_PDP_001**

**Title:** Product title on the PDP matches the title clicked in the search results

**Summary**: 

Verify that the product title displayed on the PDP matches the title of the book the user clicked on from the SRP

**Priority:** High

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for any book by title or author
3. Note the title of a book on the SRP
4. Click on the book
5. Observe the product title displayed on the PDP

**Expected Result:** 

The product title on the PDP exactly matches the title of the book that was clicked on the SRP

**Actual Result:**

The product title on the PDP exactly matches the title of the book that was clicked on the SRP

---

**TC_PDP_002**

**Title:** Switching between formats updates the price dynamically on the PDP

**Summary:** 

Verify that selecting a different format (e.g., switching from Paperback to Hardcover) updates the displayed price correctly on the PDP

**Priority:** High

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for and navigate to a PDP for a book available in multiple formats
3. Note the price displayed for the default format
4. Select a different format (e.g., Hardcover)
5. Observe the price displayed

**Expected Result:** 

The price updates dynamically to reflect the correct price for the selected format

**Actual Result:**

The price updates dynamically to reflect the correct price for the selected format

---

**TC_PDP_003**

**Title:** Add to Cart button is visible and functional for in-stock items on the PDP

**Summary:** 

Verify that the Add to Cart button is visible, enabled, and successfully adds the item to the cart for in-stock products

**Priority:** High

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for and navigate to a PDP for an in-stock book
3. Observe the Add to Cart button
4. Click the Add to Cart button
5. Observe the cart icon in the header

**Expected Result:**

 The Add to Cart button is visible,

 the item is added to the cart successfully

 the cart count in the header increments by one

**Actual Result:**

 The Add to Cart button is visible,

 the item is added to the cart successfully

 the cart count in the header increments by one

---

**TC_PDP_004**

**Title:** Clicking the author's name on the PDP redirects to a list of their other works

**Summary:**

 Verify that clicking the author's name on the PDP redirects the user to a page listing all other available works by that author

**Priority:** Medium

**Status:**  Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for and navigate to any PDP
3. Locate the author's name on the PDP
4. Click on the author's name
5. Observe the page that loads

**Expected Result:** 

The user is redirected to a page displaying all available books written by that author

**Actual Result:**

The user is redirected to a page displaying all available books written by that author

---

**TC_PDP_005 – NEGATIVE**

**Title:** Users cannot add an out of stock item to the cart via the PDP

**Summary:** 

Verify that the Add to Cart button is disabled or hidden for products that are listed as out of stock on the PDP

**Priority:** High

**Status:** Passed

**Environment**: Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for “collen”
3. Set the filter to e books and scroll down
4. Attempt to Add an unavailable item to Cart

**Expected Result:** 

The Add to Cart button is either disabled or hidden and a clear out of stock message is displayed to the user preventing them from adding the item to the cart

**Actual Result:**

The Add to Cart button is  hidden and a clear out of stock message is displayed to the user preventing them from adding the item to the cart

---

**TC_PDP_006 – NEGATIVE**

**Title:** Navigating to a PDP with an invalid Product ID displays a Product Not Found page

**Summary**:

 Verify that navigating to a PDP via a direct URL with an invalid Product ID displays a user-friendly Product Not Found error page

**Priority:** Medium

**Status:**  Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. In the browser address bar manually enter a PDP URL with an invalid Product ID (e.g., https://www.booksamillion.com/product/9999999999)
3. Press Enter and observe the page behaviour

**Expected Result:** 

The site displays a clear and user-friendly Product Not Found or 404 error page with navigation options to return to the homepage or search for another book

**Actual Result:**

The site displays a clear and user-friendly Product Not Found 

The user is given some other recommendations

---

## 5. Cart

---

**TC_CT_001**

**Title:** Adding a book to the cart increases the cart count in the header by 1

**Summary:** 

Verify that clicking the Add to Cart button on a PDP successfully adds the book to the cart and increments the cart count by 1

**Priority:** High

**Status:** Passed

**Environment:** Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Search for any book and navigate to its PDP
3. Note the current cart count displayed in the header
4. Click the Add to Cart button
5. Observe the cart count in the header

**Expected Result:** 

The cart count in the header increments by 1 immediately after the book is added and the item is visible in the cart

**TC_CT_002**

**Actual Result:**

The cart count in the header increments by 1 immediately after the book is added and the item is visible in the cart

---

**Title:** Adding the same book twice increases the quantity to 2 within the same line item

**Summary:** 

Verify that adding the same book to the cart twice updates the quantity to 2 within the same line item rather than creating a duplicate entry

**Priority:** High

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Navigate to any PDP and click Add to Cart
3. Navigate back to the same PDP and click Add to Cart again
4. Open the cart and observe the line items

**Expected Result:** 

The cart displays a single line item for the book with the quantity updated to 2 and the subtotal reflecting the correct combined price

**Actual Result:**

The cart displays a single line item for the book with the quantity updated to 2 and the subtotal reflecting the correct combined price

---

**TC_CT_003**

**Title:** Cart subtotal accurately reflects the combined price of all items

**Summary:** Verify that the subtotal displayed in the cart matches the combined price of all items added

**Priority:** High

**Status:** Passed

**Environment:** Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Add two or more different books to the cart
3. Navigate to the cart
4. Note the individual prices of each item
5. Observe the subtotal displayed

**Expected Result:** 

The subtotal accurately reflects the sum of all individual item prices in the cart with no discrepancies

**Actual Result:**

The subtotal accurately reflects the sum of all individual item prices in the cart with no discrepancies

---

**TC_CT_004**

**Title:** Removing an item from the cart successfully deletes it from the cart list

**Summary:**

 ****Verify that clicking the remove button on a cart item successfully deletes it from the cart and updates the cart count and subtotal

**Priority:** High

**Status:** Passsed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Add two books to the cart and navigate to the cart
3. Click the remove button next to one of the items
4. Observe the cart contents, cart count, and subtotal

**Expected Result:** 

The item is removed from the cart list, the cart count decreases by 1, and the subtotal updates to reflect the remaining item

**Actual Result:**

The item is removed from the cart list, the cart count decreases by 1, and the subtotal updates to reflect the remaining item

---

**TC_CT_005**

**Title:** Cart persists when the user navigates to a different page and returns

**Summary:** Verify that items added to the cart are still present when the user navigates away and returns to the cart within the same session

**Priority:** High

**Status:** Passed

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Add one or more books to the cart
3. Navigate to a different page (e.g., homepage or a category page)
4. Click the cart icon to return to the cart
5. Observe the cart contents

**Expected Result:**

 ****All previously added items are still present in the cart with the correct quantities and prices

**Actual Result:**

 ****All previously added items are still present in the cart with the correct quantities and prices

---

**TC_CT_006 – NEGATIVE**

**Title:** Checkout button is disabled when the cart is empty

**Summary**: 

Verify that the Proceed to Checkout button is disabled or hidden when the cart contains no items

**Priority:** High

**Status:** Passed

**Environment**: Windows 11

**Browser:** Microsoft Edge

1. Open https://www.booksamillion.com/
2. Navigate to the cart without adding any items
3. Observe the Proceed to Checkout button and the cart page content

**Expected Result:** 

The Proceed to Checkout button is  hidden

 The cart displays a clear empty state message saying: 

Your Shopping Cart is empty. Continue Shopping and select 'Add to Cart' to move items into your cart

**Actual Result:**

The Proceed to Checkout button is  hidden

 The cart displays a clear empty state message saying: 

Your Shopping Cart is empty. Continue Shopping and select 'Add to Cart' to move items into your cart

---

**TC_CT_007 – NEGATIVE**

**Title:** Using the browser back button after removing an item does not restore the removed item

**Summary**: 

Verify that using the browser back button after removing an item from the cart does not restore the previously removed item

**Priority**:High

**Status:** Failed

**Environment**: Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open https://www.booksamillion.com/
2. Add two books to the cart and navigate to the cart
3. Remove one item from the cart
4. Click the browser back button
5. Observe the cart contents

**Expected Result:** 

The removed item remains deleted from the cart and does not reappear after using the browser back button

**Actual Result:**

The removed item removed appears after using the browser back button
