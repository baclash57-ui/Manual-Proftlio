## User Flow

1. Validate that, upon first accessing the link, the user is prompted to complete a human verification check.

### Homepage

### Valid Scenarios

1. Verify the functionality of all elements in the homepage to ensure they are interactive.
2. Verify that clicking the company logo from any sub-page returns the user to the homepage.
3. Verify that the "Best Sellers" navigation link redirects to the correct curated list.
4. Verify that category-specific links (e.g., Manga, Kids) lead to the correct filtered galleries.
5. Verify that all images on the homepage load correctly without broken placeholders.
6. Verify that the main promotional banners redirect to their specific campaign pages.
7. Verify that the footer links (within scope) redirect to the correct informational pages.

### Invalid Scenarios

1. Verify that manual URL manipulation to an invalid category does not crash the site.
2. Verify that the navigation menu does not overlap or become unclickable on smaller screen resolutions.
3. Verify that clicking a navigation element during a slow network connection does not result in a blank white screen.
4. Verify system behavior when clicking an unavailable book

### Search & Filter

### Valid Scenarios

1. Verify that searching for a exact book title returns the specific book as the first result.
2. Verify that searching by an Author's name returns all books written by them
3. Verify that searching by a 10 or 13-digit ISBN returns the exact matching product.
4. Verify that the auto-suggestion dropdown provides relevant titles while the user types.
5. Verify that the "Sort by Newest" functionality displays the latest releases first.
6. Verify that combining multiple filters (e.g., Genre + Price Range) narrows results accurately.
7. Verify that clicking "Clear All Filters" restores the original, unfiltered search results.
8. Verify that the search results count matches the number of items displayed on the page.
9. Verify that applying a "Format" filter (e.g., Hardcover) excludes all other formats from the results.

### Invalid Scenarios:

1. Verify that searching with only special characters (e.g., `!@#$%`) displays a "No Results" message.
2. Verify that entering an excessively long string (255+ characters) in the search bar is handled gracefully.
3. Verify that searching for a non-existent ISBN displays a helpful error message.
4. Verify that the system handles "SQL Injection" attempts in the search bar without exposing database errors.
5. Verify that removing a filter that was never applied does not cause a system refresh error.
6. Verify that the "Sort" function does not break when the search result contains only one item.

### Product Description Page

### Valid Scenarios

1. Verify that the product title on the PDP matches the title clicked in the search results.
2. Verify that switching between Paperback and Hardcover updates the price dynamically.
3. Verify that the "In Stock" or "Out of Stock" status is clearly displayed for each format.
4. Verify that the product description expands and collapses correctly.
5. Verify that clicking the Author’s name on the PDP redirects to a list of their other works.
6. Verify that the ISBN and Publisher details are accurate and legible.
7. Verify that the "Related Books" or "Customers Also Bought" section displays relevant items.

### Invalid Scenarios:

1. Verify that users cannot add an "Out of Stock" item to the cart via the PDP.
2. Verify that navigating to a PDP via a direct URL with an invalid Product ID displays a "Product Not Found" page.
3. Verify that the price does not display as $0.00 for any valid book listing.
4. Verify that selecting a format that is unavailable doesn't result in a blank page.
5. Verify that the quantity selector does not allow a user to input a negative number.

### Cart:

### Valid  Scenarios:

1. Verify that adding a book to the cart increases the cart count in the header by **1**
2. .Verify that adding the same book twice increases the quantity to **2** within the same line item.
3. Verify that removing an item from the cart successfully deletes it from the list.
4. Verify that the total count price matches the actual price.
5. Verify that the cart persists when the user navigates to a different page and returns.
6. Verify that the "Proceed to Checkout" button is enabled only when there is at least one item in the cart.
7.  Verify that the cart displays the correct format (e.g., eBook) for the item added.

### Invalid Scenarios:

1. Verify that the "Checkout" button is disabled if the cart is empty.
2. Verify that the subtotal does not become negative if a discount exceeds the item price.
3. Verify that the cart does not lose items if the user's internet connection momentarily drops.
4.  Verify that manual browser "Back" button usage after removing an item doesn't resurrect the item in the cart.

### Customer Support(Live Chat) flow:

### Valid Scenarios

1. Verify the functionality and visibility of the live chat trigger across all in-scope pages (Homepage, Search, PDP, and Cart).
2. Verify that the chat session initiates successfully after providing valid mandatory information (e.g., Name and Email) in the pre-chat form.
3. Verify that the chat interface allows for the successful sending and receiving of text messages between the user and the agent.
4. Verify that the chat window and conversation history remain active and intact while the user navigates between different pages of the site.
5. Verify the functionality of the "Minimize" and "Maximize" buttons to ensure the chat can be tucked away without ending the session.
6. Verify that links sent by the support agent (such as product pages or help articles) are clickable and open correctly in a new tab.
7. Verify that clicking the "End Chat" or "Close" button successfully terminates the session and provides a confirmation prompt.

### Invalid Scenarios

1. Verify the system's behavior when a user attempts to initiate a chat outside of operational business hours (e.g., displays an "Offline" message or an email contact form).
2.  Verify that the chat input field rejects or neutralizes malicious scripts (e.g., `<script>alert('XSS')</script>`) to prevent cross-site scripting attacks.
3.  Verify that the chat interface provides a clear "Reconnecting" or "Connection Lost" notification if the user's internet drops.
4. Verify that the system prevents the upload of prohibited or dangerous file types (e.g., .exe, .bat, or excessively large files).
5. Verify that the chat widget does not overlap or prevent interaction with critical "Call to Action" buttons like "Add to Cart" or "Proceed to Checkout" on different Views.
