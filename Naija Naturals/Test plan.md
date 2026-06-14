** Test Environment**

| Field | Details |

|---|---|

| Platform | Desktop |

| Operating System | Windows 11 |

| Browser | Microsoft Edge (Latest Stable) |

| Application | NN Hair & Beauty – naijanaturals.com |

| Test Type | Functional, UI/UX, Regression |

| Test Scope | End-to-End User Journey (Homepage to Checkout – Payments OOS) |

| Prepared By | Senior QA Engineer |

| Review Date | February 18, 2026 |

**Application Overview**

NN Hair & Beauty is a Nigerian-based e-commerce platform specialising in hair care and beauty products, with a primary target audience of women. The platform offers both in-store pickup and door-to-door delivery options, enabling customers to browse, compare, and purchase a wide range of hair and beauty products from Nigeria's leading beauty retail store.

The website features a product-rich homepage with category navigation, a robust search and filter system, detailed product description pages, and a shopping cart that feeds into a checkout flow.

**Core User Flow**

1. Browsing products on the homepage and product category pages

2. Searching for products by name, brand, and description (e.g., hair spray)

3. Filtering items on the product listing page to the preferred type

4. Viewing the Product Description Page (PDP)

5. Adding items to cart

6. Payment for items

7. Tracking orders

- --

 **In-Scope Test Areas**

> **Note:** Payment processing is explicitly out of scope for this test cycle. Testing covers all user-facing functionality from the homepage through to the checkout entry point.

- --

 **1. Homepage**

- Verify that the page loads correctly and all above-the-fold elements render without visual breakage on Microsoft Edge (Windows 11)
- Confirm the header navigation bar is visible, correctly positioned, and all top-level menu items are clickable and labelled correctly
- Verify all main navigation menus expand correctly on hover or click and display the appropriate sub-menu items
- Confirm sub-menu items redirect the user to the correct corresponding category or page
- Validate that clicking the company logo from any page redirects the user back to the homepage
- Verify hero/banner images load correctly, are not broken, and display relevant promotional content
- Confirm banner CTA buttons or links redirect users to the correct destination pages
- Verify that product cards on the homepage display correctly, including product images, names, prices, and any discount/sale badges
- Confirm product category sections are clearly labelled and separated on the homepage
- Validate the visual arrangement and alignment of all page elements (images, banners, text blocks, product grids)
- Verify page responsiveness when buttons and interactive elements are clicked
- Confirm there are no broken images, placeholder text, or missing content visible on the homepage
- Validate the Best Sellers or featured product sections display correctly and are interactive
- Verify the sticky/fixed header (if present) remains visible and functional when scrolling down the page
- --

 **2. Search & Filter**

**2a. Search Functionality**

- Verify the search bar is prominently visible and accessible from the homepage and all key pages
- Confirm the search bar accepts input via keyboard and returns results on pressing Enter or clicking the search icon
- Search for products by exact product name and confirm relevant results are returned
- Search for products by brand name and confirm the results page displays the correct brand items
- Search for products by description keyword (e.g., "moisturising shampoo", "hair oil") and verify relevant results appear
- Search for products using partial keywords and verify the system handles these gracefully
- Search within a specific category (e.g., search for a spray within the Best Sellers section) and confirm results are correctly scoped
- Verify that the Search Results Page (SRP) clearly displays the search query term used
- Confirm the SRP shows the correct number of results and that items match the search intent
- Perform a search using special characters or invalid input and verify the system does not crash and displays an appropriate message
- Verify that an empty search submission is handled gracefully
- Confirm that search results are not duplicated or missing expected items

 **2b. Filter Functionality**

- Verify filter options are available and clearly labelled on both the SRP and relevant category/listing pages
- Select a single filter option and confirm the product grid updates to display only matching items
- Select multiple filter options simultaneously and verify the combined filter logic returns correctly scoped results
- Adjust the price range slider/input and confirm the product list updates accordingly
- Add a filter and then remove it, confirming the product list reverts to its previous unfiltered state
- Apply filters and then refresh the page, verifying whether filters persist (document the behaviour either way)
- Verify that filter selections do not cause page crashes or unintended layout shifts
- Confirm that when filters return zero results, a user-friendly empty state message is displayed
- Verify the Clear All Filters or equivalent reset option removes all active filters correctly
- --

 **3. Product Description Page (PDP)**

- Verify that clicking on a product image or product name correctly navigates the user to the corresponding PDP
- Confirm the PDP displays the correct product name, description, price, and images that match the product selected
- Verify the product image gallery loads correctly; if multiple images exist, confirm the user can cycle through them
- Confirm product image zoom or lightbox functionality works as expected when available
- Verify that product variant selectors (e.g., size, colour, type) are present where applicable and that selecting a variant updates the relevant content
- Confirm that the product availability or stock status is clearly displayed
- Verify the Add to Cart button is visible, enabled (for in-stock items), and functional from the PDP
- Check that product ratings, reviews, or user-generated content sections load correctly if present
- Confirm any cross-sell or upsell product recommendation sections on the PDP display relevant items correctly
- Validate breadcrumb navigation on the PDP reflects the correct path and each breadcrumb link is functional
- Verify that navigating back from the PDP returns the user to the correct previous page
- --

**4. Cart Section**

- Verify that a user can successfully add items to the cart from the PDP
- Verify that items can be added to the cart from the Search Results Page (SRP)
- Verify that items can be added to the cart from product recommendation sections across the site
- Confirm the cart icon/count badge updates immediately after an item is added
- Verify that adding the same product multiple times updates the quantity correctly
- Open the cart and verify that the subtotal accurately reflects the combined price of all items
- Confirm the user can increase or decrease item quantities within the cart and that the subtotal updates accordingly
- Confirm the user can remove individual items from the cart and that both the cart count and subtotal update correctly
- Verify cart behaviour when multiple different items are added
- Verify the cart persists items correctly if the user navigates away and returns within the same session
- Confirm that the cart displays an appropriate empty state when all items have been removed
- Verify the Proceed to Checkout button is visible, functional, and navigates the user to the checkout entry page
- --

**5. Product Listing & Category Pages**

- Verify that navigating to a category from the main menu loads the correct product listing page
- Confirm that all products displayed within a category page are correctly assigned to that category
- Verify that pagination or infinite scroll loads additional products correctly without duplicating or skipping items
- Confirm product cards on listing pages display correct information (name, price, image, sale badge where applicable)
- Verify the default sort order of products on category pages and confirm it is applied correctly
- Confirm sort order options (if available) function correctly and reorder the product grid as expected

**Entry & Exit Criteria**

 **Entry Criteria**

The following conditions must be met before test execution begins:

- The test environment is accessible and stable
- Microsoft Edge (latest stable version) is installed and verified on the Windows 11 test machine
- The test plan has been reviewed and signed off by the relevant stakeholder(s)
- All in-scope features and pages are deployed and available in the test environment
- Test cases and checklists have been prepared and are ready for execution
- Any required test data (e.g., product names, search keywords, price ranges) has been identified and documented
- No P1 (critical) blocking defects exist in the environment that would prevent testing from starting
- The QA engineer has been granted sufficient access to the site

**Exit Criteria**

Testing will be considered complete when the following conditions are satisfied:

- 100% of in-scope test cases have been executed at least once
- All critical (P1) and high-severity (P2) defects have been resolved and re-tested successfully
- No open P1 defects remain unresolved at the time of sign-off
- A minimum of 90% of all test cases have passed
- A test summary report has been produced outlining total tests executed, pass/fail counts, defect counts by severity, and any known risks
- Regression testing has been completed on any area affected by bug fixes applied during the test cycle
- Stakeholder sign-off has been obtained on the test summary report
- --

 **Out-of-Scope Areas**

- Payment processing and payment gateway integrations
- User login and registration functionality
- Footer links and footer navigation items
- Social media handle links and integrations
- UK store variant
- Newsletter subscription and email marketing functionality
- Contact Us page and customer support forms
- Order tracking post-purchase
- Wishlist / Save for Later functionality
- User account dashboard (order history, saved addresses, profile management)
- Third-party integrations (live chat widgets, analytics scripts, ad pixels)
- Mobile and tablet responsiveness (Desktop – Windows 11 / Microsoft Edge only)
- Cross-browser compatibility testing (Edge only for this cycle)
- Performance and load testing
- Accessibility (WCAG) compliance testing
- SEO metadata and structured data validation
- --

** Assumptions & Dependencies**

- The test environment is the live production site at naijanaturals.com or a designated staging environment that mirrors it closely
- Microsoft Edge is updated to the latest stable release prior to test execution
- Test execution is performed on a Windows 11 desktop machine with a minimum 1920x1080 screen resolution
- All in-scope product pages, categories, and cart functionality are accessible without requiring user authentication unless otherwise noted
- Product data (names, prices, images) is treated as reference data and is assumed to be accurate for validation purposes
- Any bugs discovered in OOS areas will be logged but not prioritised in this cycle
- --

** Document Sign-Off**

| Field | Details |

|---|---|

| Prepared By | Japhet Obinna Prosper |

| Reviewed By | |

| Approved By | |

| Version | 1.0 |

| Date | February 18, 2026 |

| Status | Draft – Pending Review |
