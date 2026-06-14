**Project Summary — CandyStore.com Testing Exercise**

CandyStore.com is a large e-commerce website focused on the purchase and distribution of various candy products. Overall, the application performs well across its core user flows — browsing, searching, filtering, and cart management — with the majority of test cases returning a Pass status. The site is functional, stable, and provides a good user experience for the most part.

---

**Test Results Overview**

Five test cases were executed across the cart and search functionalities, all of which passed successfully:

| Test Case ID | Title | Status |
|---|---|---|
| TC_CART_001 | Add product to cart from product listing page | Pass |
| TC_CART_002 | Update product quantity in cart | Pass |
| TC_CART_003 | Cart retains items after page refresh | Pass |
| TC_CART_004 | Remove product from cart | Pass |
| TC_SEARCH_001 | Search returns relevant results for valid keyword | Pass |

The cart section in particular proved to be solid and reliable — products are added correctly, quantities update accurately, the cart persists after a page refresh, and item removal works as expected with no errors or unexpected behavior.

---

**Bugs Found**

Four bugs were identified and reported during the testing exercise:

**1. Candy items with different colors displayed when searching by a particular color (Severity: Low)**
When a user filters candy by a specific color (e.g., green) and navigates to page two and three of the Product Listing Page, candy items of a different color (blue) appear in the results. This affects the accuracy of the color filter feature.

**2. BG-FT_001 — Filter option is not responsive (Severity: Medium)**
The best selling filter option on the submenu page is completely unresponsive. When a user clicks on it, nothing happens and no dropdown menu is displayed, making the filter feature unusable.

**3. BG-FT_002 — Filter price option displays negative values (Severity: Medium)**
The price filter allows users to set negative values by clicking and holding the downward arrow on the min or max price input. This is unintended behavior as price values should not go below zero.

**4. BG-PlP_002 — Product is missing an image (Severity: Low)**
On the cookie and cookie dough flavour listing page, the product "Clif Bar-Buildes cookies" is missing its image, leaving it without a visual representation on the Product Listing Page.

---

**Overall Assessment**

CandyStore.com is a well-built e-commerce application that handles its core functionalities reliably. The cart and search features work smoothly with no critical failures recorded. The bugs found are low to medium in severity and do not break the core experience, however the unresponsive filter and negative price value issues are worth prioritizing as they directly impact product discovery which is a key part of the user journey.

---
