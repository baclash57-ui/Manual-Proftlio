### **1. Home Page Navigation**

**Valid Scenarios:**

- Navigate to the home page via URL and verify it loads successfully.
- Verify all main menu and submenu links are clickable and redirect correctly.
- Verify the homepage displays banners, featured products, and promotions correctly.

**Invalid Scenarios:**

- Access the homepage while offline and verify proper error notification.
- Refresh the home page multiple times

---

### **2. Search for a Product**

**Valid Scenarios:**

- Enter a valid product name and verify the correct results appear.
- Search with a product by category (brand , color, flavor, bestselling, etc) and verify the correct product page loads.

**Invalid Scenarios:**

- Enter random strings or special characters and verify the system handles them without crashing.
- Search for a product that doesn't exist and verify an appropriate "No results found" message appears.
- Submit an empty search query and verify the system prevents it or shows a warning.

---

### **3. Filter Products**

**Valid Scenarios:**

- Apply a price filter and verify only products within the selected range are displayed.
- Filter by price, availability, colors, etc  and verify results match the criteria.
- Combine multiple filters and verify results are correct.
- Clear filters and verify all products are displayed again.

**Invalid Scenarios:**

- Apply conflicting filters (e.g., price below $50 and above $1,000) and verify proper messaging or empty results.
- Select invalid filter values (if possible via URL manipulation) and ensure the system doesn't crash.

---

### **4. Browse Products by Category**

**Valid Scenarios:**

- Click a category from the main menu and verify all products in that category are displayed.
- Navigate through subcategories and verify results match the selection.

**Invalid Scenarios:**

- Click a non-existent category (via URL manipulation) and verify a 404 or proper error page appears.
- Load category pages while offline and verify appropriate messaging.

---

### **5. Add Items to Cart**

**Valid Scenarios:**

- Add a single product to the cart and verify it appears with the correct quantity and price.
- Add multiple products to the cart and verify all items appear correctly.
- Update the quantity in the cart and verify the total price updates correctly.
- Remove items from the cart and verify it updates.

**Invalid Scenarios:**

- Add a product with a quantity exceeding available stock and verify proper validation or error message.
- Add a product to the cart while offline and verify the system prevents it or shows a message.
