# NN Hair & Beauty – Test Scenarios

---

## 1. Homepage

- Verify that the homepage loads successfully
- Verify that the homepage banner images load and display correctly
- Verify that the main navigation menu is visible and accessible
- Verify that hovering/clicking on a menu item expands the correct sub-menu
- Verify that clicking a sub-menu item redirects to the correct page
- Verify that clicking the company logo from any page returns the user to the homepage
- Verify that all product cards on the homepage display correctly
- Verify that clicking a product card navigates to the correct PDP
- Verify that the Best Sellers section loads and displays the correct products
- Verify that banner CTA buttons redirect to the correct destination
- Verify that there are no broken images on the homepage
- Verify that the sticky header remains visible while scrolling
- Verify that all homepage elements are correctly aligned and arranged
- Verify that clicking any interactive button produces the correct page response

---

## 2. Search & Filter

### Search

- Verify that the search bar is visible and accessible from the homepage
- Verify that searching by exact product name returns the correct results
- Verify that searching by brand name returns the correct results
- Verify that searching by keyword/description returns relevant results
- Verify that searching with a partial keyword returns relevant results
- Verify that the Search Results Page displays the search term used
- Verify that search results match the query entered
- Verify that searching within a specific category returns correctly scoped results
- Verify that searching with special characters does not crash the page
- Verify that submitting an empty search is handled gracefully
- Verify that search results contain no unexpected duplicates

### Filter

- Verify that filter options are visible and accessible on the SRP
- Verify that selecting a single filter updates the product grid correctly
- Verify that selecting multiple filters returns correctly scoped results
- Verify that adjusting the price range updates the product list accordingly
- Verify that removing a filter reverts the product list to its previous state
- Verify that clearing all filters resets the page correctly
- Verify that filters do not persist after a page refresh
- Verify that applying filters with no matching results displays an empty state message
- Verify that applying filters does not cause any page crashes or layout issues

---

## 3. Product Description Page (PDP)

- Verify that clicking a product image navigates to the correct PDP
- Verify that clicking a product name navigates to the correct PDP
- Verify that the product name on the PDP matches the product selected
- Verify that the product price on the PDP matches the product selected
- Verify that the product description on the PDP matches the product selected
- Verify that the product image(s) on the PDP load correctly
- Verify that the user can cycle through multiple product images where available
- Verify that the image zoom or lightbox feature works correctly where available
- Verify that product variant selectors are present and functional where applicable
- Verify that selecting a variant updates the product details accordingly
- Verify that the stock/availability status is clearly displayed
- Verify that the Add to Cart button is visible and functional
- Verify that product recommendations on the PDP display correctly
- Verify that breadcrumb navigation on the PDP is correct and functional
- Verify that navigating back from the PDP returns the user to the correct previous page

---

## 4. Cart Section

- Verify that a user can add an item to the cart from the PDP
- Verify that a user can add an item to the cart from the SRP
- Verify that a user can add an item to the cart from the product recommendation section
- Verify that the cart count updates immediately after an item is added
- Verify that adding the same product multiple times updates the quantity correctly
- Verify that the cart subtotal reflects the correct total price of all items
- Verify that the user can increase item quantity within the cart
- Verify that the user can decrease item quantity within the cart
- Verify that the user can remove an item from the cart
- Verify that the cart count and subtotal update correctly after removing an item
- Verify that the cart retains items after the user navigates away and returns
- Verify that the cart displays an empty state message when all items are removed
- Verify that the cart behaves correctly when multiple different items are added
- Verify that the Proceed to Checkout button is visible and functional

---

## 5. Product Listing & Category Pages

- Verify that clicking a category from the navigation loads the correct listing page
- Verify that all products on a category page belong to the correct category
- Verify that product cards display the correct name, price, and image
- Verify that sale or discount badges display correctly where applicable
- Verify that pagination loads the next set of products correctly
- Verify that infinite scroll loads additional products without duplicating items
- Verify that the default sort order is applied correctly on page load
- Verify that changing the sort order reorders the product grid correctly

---

## 6. Checkout (Pre-Payment)

- Verify that clicking Proceed to Checkout from the cart navigates to the checkout page
- Verify that the checkout page displays a correct summary of all items in the cart
- Verify that the item names, quantities, and prices on the checkout page match the cart
- Verify that the order subtotal on the checkout page matches the cart subtotal
- Verify that the user can enter a delivery address on the checkout page
- Verify that the delivery address form validates required fields correctly
- Verify that the user can select a delivery method where options are available
- Verify that selecting a delivery method updates the order total accordingly
- Verify that any applicable delivery fees are clearly displayed
- Verify that a promo/discount code field is present and accepts input
- Verify that the checkout page displays a clear order summary before payment
- Verify that the user cannot proceed past checkout without completing required fields
- Verify that navigating back from checkout returns the user to the cart with items intact

---
