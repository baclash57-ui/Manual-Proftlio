# NN Hair & Beauty – Test Cases

---

## 1. Homepage

---

**TC_HP_001**

**Title**: Homepage loads successfully on Microsoft Edge

**Summary:** Verify that the homepage loads completely with all elements visible and functional when navigated to on Microsoft Edge (Windows 11)

**Priority:** High

**Status: Passed**

**Environment:** Windows 11 

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Click on the  naijanaturals.com
2. Observe the page load

**Expected Result:** The homepage loads fully with all images, banners, navigation, and product cards visible and no broken elements

**Actual Result:**

The homepage loads fully with all images, banners, navigation, and product cards visible and no broken elements

---

**TC_HP_002**

**Title:** Main navigation menu redirects to the correct page

**Summary:** Verify that clicking a top-level navigation menu item and selecting a sub-menu option redirects the user to the correct page

**Priority:** High

**Status: Passed**

**Environment:** Windows 11 

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Click on the  naijanaturals.com
2. On the homepage, hover or click on a top-level menu item
3. Observe the sub-menu that appears
4. Click on a sub-menu item

**Expected Result:** The user is redirected to the correct category or product listing page that matches the sub-menu item clicked

**Actual Result:**

The user is redirected to the correct category or product listing page that matches the sub-menu item clicked

---

**TC_HP_003**

**Title:** Company logo redirects user back to the homepage

**Summary:** Verify that clicking the company logo from any page on the site returns the user to the homepage

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11 

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Click on the  naijanaturals.com
2.  On the homepage, click on any sub-menu item to move to another page
3. Once on the new page, click the company logo in the header

**Expected Result:** 

The user is redirected back to the homepage regardless of which page they were on

**Actual Result:**

 The user is redirected back to the homepage regardless of which page they were on

---

---

**TC_HP_004**

**Title**: Banner CTA button redirects to the correct destination

**Summary:** Verify that clicking a Call-to-Action button within a homepage banner redirects the user to the correct page

**Priority**: Medium

**Status: passed**

**Environment:** Windows 11 

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Navigate to the homepage
2. Locate a CTA button within the hero/banner section
3. Click the CTA button

**Expected Result:** 

The user is redirected to the correct page as indicated by the banner content

**Actual Result:**

The user is redirected to the correct page 

---

**TC_HP_005**

**Title:** Broken images do not appear on the homepage

**Summary:** Verify that no broken or missing images are present anywhere on the homepage

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11 

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open the naijanaturals.com link
2. On the homepage, scroll through the entire page from top to bottom
3. Observe all images including banners, product cards, and section images

**Expected Result:**

 All images load correctly with no broken image icons, blank spaces, or placeholder images visible

**Actual Result:**

All images load correctly with no broken image icons, blank spaces, or placeholder images visible

---

---

**TC_HP_0006 – NEGATIVE**

**Title:** Homepage does not crash when navigated to with a slow network connection

**Summary:** Verify that the homepage degrades gracefully and does not crash or display unformatted content when loaded under poor network conditions

**Priority**: Low

**Status: Pass**

**Environment:** Windows 11 

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open Microsoft Edge DevTools (F12)
2. Navigate to the Network tab and set throttling to "Slow 3G/4G"
3. Navigate to naijanaturals.com
4. Observe the page load behaviour

**Expected Result:** 

The homepage loads fully 

The homepage displays a graceful loading state without crashing or showing broken layouts

**Actual Result:**

The homepage loads gracefully

The homepage displays a graceful loading state without crashing or showing broken layouts

---

---

## 2. Search & Filter

**TC_SF_001**

**Title:** Searching by exact product name returns correct results

**Summary:** Verify that entering an exact product name into the search bar returns the correct and relevant products on the SRP

**Priority:** High

**Status: Passed**

**Environment:** Windows 11 

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open the naijanaturals.com link
2. On the homepage, click on the search bar
3. Type an exact product name (e.g., "Shea Moisture Shampoo")
4. Press Enter or click the search icon

**Expected Result**:

When the product is available:

 The SRP displays products that match the exact product name entered and the search term is visible on the results page

When the item is unavailable:

User receives a message telling them item unavailable

**Actual Result:**

If the product is available:

The search term is visible on the results page

The SRP displays products that match the exact product name entered and the search term is visible on the results page

The user is given other products that was bought along with the product

When the item is unavailable:

User receives a message telling them item  is unavailable

---

**TC_SF_002**

**Title:** Searching by brand name returns correct results

**Summary:** Verify that entering a brand name into the search bar returns all products associated with that brand

**Priority:** High

**Status: Passed** 

**Environment:** Windows 11 

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Navigate to the homepage
2. Click on the search bar
3. Type a known brand name (e.g., "ORS")
4. Press Enter or click the search icon

**Expected Result:** 

The SRP shows gracefully

The SRP displays only products belonging to the searched brand with no irrelevant items shown

**Actual Result:**

 The SRP displays only products belonging to the searched brand 

---

**TC_SF_003**

**Title:** Applying a single filter updates the product grid correctly

**Summary:** Verify that selecting one filter option on the SRP updates the product listing to show only items matching that filter

**Priority:** High

**Status: Passed** 

**Environment**: Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Click on the search bar and search for a product
3. Click the filter options panel
4. Select one filter option (e.g., a product category or type)
5. Observe the product grid

**Expected Result:**

 The product grid updates gracefully

Only items that match the selected filter option are displayed

**Actual Result:**

 The product grid updates gracefully

Only items that match the selected filter option are displayed

---

**TC_SF_004**

**Title:** Adjusting price range filter updates results correctly

**Summary:** Verify that setting a price range on the SRP filters the product list to show only items within the selected price band

**Priority:** High

**Status: Failed**

**Environment:** Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Click on the search bar and search for a product
3. Click the filter options panel
4. Select a price range  filter option
5. Observe the product grid

**Expected Result:**

 Only products that fall within the specified price range are displayed in the product grid

**Actual Result:**

The FRP displays products unrelated to the product searched when the filter option is high

---

**TC_SF_005**

**Title:** Removing a filter reverts the product list to its unfiltered state

**Summary:** Verify that deselecting an active filter returns the product grid back to the full unfiltered results

**Priority:** Medium

**Status: Passed**

**Environment**: Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Perform a search and apply one filter
3. Confirm the filtered results are displayed
4. Deselect or remove the active filter
5. Observe the product grid

**Expected Result:** 

The product grid reverts to showing the full unfiltered search results

**Actual Result:**

The product grid returns to showing the original  unfiltered search results

---

**TC_SF_006 – NEGATIVE**

**Title:** Searching with an invalid or gibberish keyword returns a no results message

**Summary:** Verify that entering an invalid search term does not crash the page and instead displays a user-friendly empty state message

**Priority**: Medium

**Status: Pass** 

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Click on the search bar
3. Type a gibberish term (e.g., "xyzabc123!!!")
4. Press Enter or click the search icon

**Expected Result:** The SRP displays a clear and user-friendly message indicating no results were found with no page crash or error

**Actual Result:** The User receives message saying: 

“No products were found matching your selection” 

---

**TC_SF_007 – NEGATIVE**

**Title:** Submitting an empty search does not crash the page

**Summary:** Verify that pressing Enter or clicking the search icon without entering any text is handled gracefully

**Priority:** Medium

**Status: passed** 

**Environment:** Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Click on the search bar without typing anything
3. Press Enter or click the search icon
4. Observe the page behaviour

**Expected Result:** 

Nothing happens

The User stays on the homepage

**Actual Result:** 

Nothing happens

The User stays on the homepage

---

**TC_SF_008 – NEGATIVE**

**Title:** Applying filters that return zero results displays an empty state

**Summary:** Verify that combining filters in a way that produces no matching products shows an appropriate empty state rather than a broken page

**Priority:** Low

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Perform a search on the SRP
3. Apply multiple filters that are unlikely to have matching products together
4. Observe the product grid

**Expected Result:** 

A clear and user-friendly empty state message is displayed informing the user that no products match the selected filters

**Actual Result:**

A clear and user-friendly empty state message is displayed informing the user that no products match the selected filters

---

---

## 3. Product Description Page (PDP)

---

**TC_PDP_001**

**Title:** Clicking a product image takes User to the correct PDP

**Summary:** Verify that clicking on a product image from the homepage or SRP takes the user to the correct Product Description Page

**Priority:** High

**Status: Pass**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Navigate to the homepage or SRP
3. Note the name of a product
4. Click on the product image

**Expected Result:** 

The user is taken to the PDP and the product name, price, and images match the product that was clicked

**Actual Result:**

The  User is taken to the PDP of the product clicked

The content of the PDP correspond with the product

---

---

**TC_PDP_002**

**Title:** Selecting a product variant updates the product details

**Summary:** Verify that selecting a different variant (e.g., colour, type) on the PDP updates the relevant product information accordingly

**Priority:** High

**Status: Pass**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Scroll  down to the Products Listing section in the homepage
3. Click on any product  
4. Select a different variant from the available options
5. Observe the product price, image, and availability

**Expected Result:** 

The product details update correctly to reflect the selected variant including price and image where applicable

**Actual Result:**

The product details update correctly to reflect the selected variant including price and image where applicable

---

**TC_PDP_003**

**Title:** Add to Cart button is functional from the PDP

**Summary:** Verify that clicking the Add to Cart button on the PDP successfully adds the item to the cart when items are available

**Priority:** High

**Status: Pass**

**Environment:** Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Scroll  down to the Products Listing section in the homepage
3. Click on any product  
4. On the PDP, click the Add to Cart button

**Expected Result**

The item is added to the cart, the cart count badge updates, and a confirmation message or indicator is displayed

**Actual Result:**

The item is added to the cart, the cart count badge updates, and a confirmation message or indicator is displayed

---

---

**TC_PDP_004 – NEGATIVE**

**Title**: Navigating back from the PDP returns the user to the correct previous page

**Summary:** Verify that using the browser back button from the PDP returns the user to the page they came from

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Perform a search to land on the SRP
3. Click on a product to open the PDP
4. Click the browser back button

**Expected Result:** 

The user is returned to the SRP with the previous search results still displayed

**Actual Result:**

The user is returned to the SRP with the previous search results still displayed

The user can navigate through the webpage with the browser navigations 

---

## 4. Cart Section

---

**TC_CT_001**

**Title:** User can add an item to the cart from the PDP

**Summary:** Verify that clicking the Add to Cart button on a PDP successfully adds the product to the cart

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Click on any product 
3. On the PDP, click the Add to Cart button
4. Observe the cart icon

**Expected Result:** The item is added to the cart and the cart count badge increments by one

**Actual Result:**

 The item is added to the cart and the cart count badge increments by one

---

**TC_CT_002**

**Title:** Cart subtotal reflects the correct total price of all items

**Summary:** Verify that the subtotal displayed in the cart accurately matches the combined price of all items added

**Priority**: High

**Status: Passed**

**Environment**: Windows 11

**Browser**: Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Add two or more items to the cart from the PDP
3. Navigate to the cart
4. Observe the subtotal amount displayed

**Expected Result:** 

The subtotal matches the sum of the individual prices of all items currently in the cart

**Actual Result:**

The subtotal matches the sum of the individual prices of all items currently in the cart

---

**TC_CT_003**

**Title:** User can increase and decrease item quantity in the cart

**Summary:** Verify that the quantity of an item in the cart can be adjusted and that the subtotal updates accordingly

**Priority:** High

**Status: Passed** 

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Add an item to the cart and navigate to the cart
3. Click the increase quantity button and observe the subtotal
4. Click the decrease quantity button and observe the subtotal

**Expected Result:** 

The item quantity updates correctly and the subtotal recalculates accurately after each adjustment

**Actual Result:**

The item quantity updates correctly and the subtotal recalculates accurately after each adjustment

---

**TC_CT_004**

**Title:** User can remove an item from the cart

**Summary**: Verify that removing an item from the cart updates the cart count and subtotal correctly

**Priority:** High

**Status: Pass**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Add an item to the cart and navigate to the cart
3. Click the remove button next to one item
4. Observe the cart count and subtotal

**Expected Result:** 

The item is removed, the cart count decreases by one, and the subtotal updates to reflect the remaining item(s)

**Actual Result:**

The item is removed, the cart count decreases by one, and the subtotal updates to reflect the remaining item(s)

---

**TC_CT_005**

**Title:** Cart retains items after navigating away and returning

**Summary:** Verify that items added to the cart are still present when the user navigates to another page and returns to the cart within the same session

**Priority:** High

**Status: Pass**

**Environment:** Windows 11

**Steps to Reproduce:**

1. Open http://naijanaturals.com/
2. Add one or more items to the cart
3. Navigate to a different page (e.g., homepage or a category page)
4. Navigate back to the cart

**Expected Result:** 

All previously added items are still present in the cart with correct quantities and prices

**Actual Result:**

All previously added items are still present in the cart with correct quantities and prices

---
