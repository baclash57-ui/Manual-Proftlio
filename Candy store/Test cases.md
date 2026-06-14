### Test Case ID

TC_CART_001

### Test Case Title

Add product to cart from product listing page

---

### Preconditions

- User is on the homepage
- Product listing page is accessible
- At least one product is available for purchase
- Cart is empty

---

### Test Steps

1. On the homepage, navigate to a product listing page
2. Click on a product, this opens the description page 
3. Click the **Add to Cart** button for the product
4. Observe cart icon or cart confirmation indicator
5. Open the cart

---

### Expected Result

- Product is successfully added to the cart
- Cart icon updates to reflect added item
- Correct product name appears in cart
- Correct default quantity (e.g., 1) is displayed
- No page errors or unexpected redirects occur

---

### Actual Result

- Product is successfully added to the cart
- Cart icon updates to reflect added item
- Correct product name appears in cart
- Correct default quantity (e.g., 1) is displayed
- No page errors or unexpected redirects occur

---

### Status

 Pass 

---

### Notes

- Verify behavior without navigating to product detail page
- Observe UI feedback (toast message, cart count update)

### Test Case ID

TC_CART_002

### Test Case Title

Update product quantity in cart

---

### Preconditions

- User has added at least one product to the cart
- Cart page is accessible
- Product quantity is set to default value (e.g., 1)

---

### Test Steps

1. Open the cart page
2. Locate the quantity selector for the product
3. Increase the product quantity (e.g., from 1 to 2)
4. Observe cart update behavior
5. Review cart summary (item count and subtotal)

---

### Expected Result

- Product quantity updates successfully
- Cart reflects the updated quantity
- Subtotal updates correctly based on new quantity
- No page refresh or errors occur
- Cart remains stable and usable

---

### Actual Result

- Product quantity updates successfully
- Cart reflects the updated quantity
- Subtotal updates correctly based on new quantity
- No page refresh or errors occur
- Cart remains stable and usable

---

### Status

Pass

---

### Notes

- Observe whether quantity updates automatically or requires confirmation
- Watch for UI lag, incorrect totals, or reset behavior

### Test Case ID

TC_CART_003

### Test Case Title

Cart retains items after page refresh

---

### Preconditions

- User has added at least one product to the cart
- Cart page is accessible
- Cart contains at least one item with quantity ≥ 1

---

### Test Steps

1. Open the cart page
2. Confirm product(s) are visible in the cart
3. Refresh the browser page
4. Observe the cart contents after reload

---

### Expected Result

- Cart retains previously added product(s)
- Product quantity remains unchanged
- Cart subtotal remains accurate
- No loss of cart data occurs
- No error messages are displayed

---

### Actual Result

- Cart retains previously added product(s)
- Product quantity remains unchanged
- Cart subtotal remains accurate
- No loss of cart data occurs
- No error messages are displayed

---

### Status

Passed

### Test Case ID

TC_CART_004

### Test Case Title

Remove product from cart

---

### Preconditions

- User has added at least one product to the cart
- Cart page is accessible

---

### Test Steps

1. Open the cart page
2. Locate the remove option for a product
3. Click the remove option
4. Observe the cart contents and price in the subtotal

---

### Expected Result

- Selected product is removed from the cart
- Cart item count updates correctly
- Cart subtotal updates accordingly
- If the last item is removed, cart displays an empty state message
- No UI errors or unexpected behavior occur

---

### Actual Result

- Selected product is removed from the cart
- Cart item count updates correctly
- Cart subtotal updates accordingly
- If the last item is removed, cart displays an empty state message
- No UI errors or unexpected behavior occur

---

### Status

 Pass 

### Test Case ID

TC_SEARCH_001

### Test Case Title

Search returns relevant results for valid keyword

---

### Preconditions

- Website search functionality is available
- Products exist that match the search keyword
- User is on the homepage or any page with search access

---

### Test Steps

1. Locate the search input field
2. Enter a valid product-related keyword (e.g., Gummy bears)
3. Click on the search icon
4. Observe the search results page

---

### Expected Result

- Search results page is displayed
- Returned products are relevant to the entered keyword
- Product names or descriptions contain the keyword or closely related terms
- No unrelated products are shown
- Page loads without errors or broken layout

---

### Actual Result

- Search results page is displayed
- Returned products are relevant to the entered keyword
- Product names or descriptions contain the keyword or closely related terms
- No unrelated products are shown
- Page loads without errors or broken layout

---

### Status

 Pass 

### Test Case ID

TC_FILTER_001

### Test Case Title

Filter updates search results correctly

---

### Preconditions

- Products listing page is displayed
- Multiple products are available in Products listing page
- Filter options (e.g., category, flavor, color, brand, price) are visible and selectable

---

### Test Steps

1. On the PLP, Perform a search using a valid keyword
2. Confirm multiple products are displayed in the results
3. Select more than one available filter option (e.g., Category or Flavor)
4. Observe the updated search results
5. Clear or reset the applied filter

---

### Expected Result

- Search results update according to the selected filter
- Only products matching the filter criteria are displayed
- Result count updates correctly
- Filter state is clearly indicated in the UI
- Clearing the filter restores the original result set
- No page errors or layout issues occur

---

### Actual Result

- Search results update according to the selected filter
- The price filter changes after the user exceeds $299 when selecting filter options.
- Only products matching the filter criteria are displayed
- Result count updates correctly
- Filter state is clearly indicated in the UI
- The user cannot clear the price filter

---

### Status

FAILED
