# Booking.com — Test Cases

**Environment:** Windows 11

**Tester Location:** Nigeria

**Test Type:** Manual Functional Testing

---

# HOMEPAGE

---

## General Page Behaviour

---

**Test Case ID:** TC_001

**Title:** Verify that the homepage loads successfully

**Summary:** 

Verify that all elements on the homepage load correctly when the user navigates to booking.com

**Priority:** Critical

**Status: PASSED**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Open the browser
2. Navigate to booking.com

**Expected Result:** 

The homepage loads successfully with all sections, images, headers, and the search bar visible

**Actual Result:**

The homepage loads successfully with all sections, images, headers, and the search bar visible

---

**Test Case ID:** TC_002

**Title:** Verify the behaviour of the homepage when refreshed multiple times

**Summary:**

 Verify that the homepage remains stable and consistent after multiple refreshes

**Priority:** Medium

**Status: PASSED**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Refresh the page repeatedly using the browser refresh button or Ctrl+R

**Expected Result:**

 The homepage reloads correctly each time without breaking the layout or losing content

**Actual Result:**

The homepage reloads correctly each time without breaking the layout or losing content

---

**Test Case ID:** TC_003

**Title:** Verify homepage behaviour across different screen sizes

**Summary:** 

Verify that the homepage is responsive and displays correctly on different screen sizes and viewports

**Priority:** High

**Status: PASSED**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Resize the browser window to simulate desktop, tablet, and mobile viewports
3. Observe the layout and elements at each size

**Expected Result:** 

The homepage layout adjusts correctly at each viewport size with no overlapping or broken elements

**Actual Result:**

The homepage layout adjusts correctly at each viewport size with no overlapping or broken elements

---

**Test Case ID:** TC_004

**Title:** Verify that clicking on images or banners on the homepage navigates to the correct page

**Summary:** 

Verify that any clickable image or banner on the homepage redirects the user to a relevant page

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Identify a clickable image or banner on the homepage
3. Click on it
4. Observe the page the user is redirected to

**Expected Result:** 

The user is redirected to a page that is relevant to the image or banner that was clicked

**Actual Result:**

The User is redirected to a the description page of the picture that was clicked

---

**Test Case ID:** TC_005

**Title:** Verify that clicking on navigation headers redirects the user to the correct page

**Summary:** 

Verify that all header navigation links on the homepage function correctly and lead to the right sections

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Click on each header navigation item one at a time
3. Observe where each link redirects the user

**Expected Result:**

Each header navigates the user to the correct and expected page or section

**Actual Result:**

Each header navigates the user to the correct page when clicked On

---

## Search & Filter

---

**Test Case ID:** TC_006

**Title:** Verify that the user can search for a valid destination using the search bar

**Summary:** 

Verify that entering a valid destination in the search bar returns relevant results

**Priority:** Critical

**Status :Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Click on the search bar
3. Type a valid destination e.g. “Lagos, Nigeria”
4. Select a suggestion from the autocomplete dropdown

1. Provide valid dates and Occupants number
2. Click the Search button

**Expected Result:** 

The user is taken to a search results page showing properties relevant to the entered destination

**Actual Result:**

The user is Redirected to a search results page showing properties relevant to the entered destination

---

**Test Case ID:** TC_007

**Title:** Verify that the user cannot select a past date as a check-in date

**Summary:** 

Verify that the date picker prevents the user from selecting dates that have already passed

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Click on the check-in date field
3. Attempt to select a date that is in the past

**Expected Result:** 

Past dates are greyed out and cannot be selected

**Actual Result:**

Past dates are greyed out 

User cannot select a past date

---

**Test Case ID:** TC_008

**Title:** Verify that the user can select a long date range for a trip

**Summary:** 

Verify that the date picker allows the user to select an extended stay duration

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Click on the check-in date field
3. Select a check-in date
4. Select a check-out date that is several months ahead

**Expected Result:** 

The date picker accepts the long date range and reflects it correctly in the search fields

**Actual Result:**

The date picker accepts the long date range and reflects it correctly in the search fields

---

**Test Case ID:** TC_009

**Title:** Verify that the user can change the number of occupants and rooms

**Summary:** 

Verify that the guest and room count selector functions correctly

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Click on the guests and rooms field
3. Increase and decrease the number of adults, children, and rooms using the provided controls

**Expected Result:** 

The guest and room count updates correctly and is reflected in the search query

**Actual Result:**

The guest and room count updates correctly and is reflected in the search query

---

**Test Case ID:** TC_010

**Title:** Verify that the search results page items match the entered search query

**Summary:** 

Verify that results displayed on the search results page are relevant to the destination and dates entered

**Priority:** Critical

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Enter a valid destination, check-in date, check-out date, and guest count
3. Click Search
4. Review the results displayed on the search results page

**Expected Result:** 

All results on the search results page are relevant to the destination and dates that were entered

**Actual Result:**

All results on the search results page are relevant to the valid destination and dates that were entered

The user receives a message when they enter invalid  destinations and is given other alternatives.

---

**Test Case ID:** TC_011

**Title:** Verify that the user can add multiple filters on the search results page

**Summary:** 

Verify that applying multiple filters simultaneously narrows down the search results correctly

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. On the search results page, apply one filter e.g. property type
3. Apply a second filter e.g. guest rating
4. Apply a third filter e.g. price range
5. Observe the results after each filter is applied

**Expected Result:**

 The search results update correctly each time a filter is added and reflect all applied filters simultaneously

**Actual Result:**

 The search results update correctly each time a filter is added and reflect all applied filters simultaneously

---

**Test Case ID:** TC_012

**Title:** Verify that the user can remove a single filter after applying it

**Summary:** 

Verify that removing one filter from the search results page updates the results correctly

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. Apply at least two filters on the search results page
3. Remove one of the applied filters
4. Observe the updated results

**Expected Result:** 

The removed filter is no longer active and the search results update to reflect the remaining filters

**Actual Result:**

The removed filter is no longer active and the search results update to reflect the remaining filters

---

**Test Case ID:** TC_013

**Title:** Verify that the user can remove multiple filters from the search results page

**Summary:** 

Verify that all applied filters can be removed and the results return to their unfiltered state

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. Apply multiple filters on the search results page
3. Remove each filter one by one
4. Observe the results after all filters have been removed

**Expected Result:** 

All filters are removed successfully and the search results return to their original unfiltered state

**Actual Result:**

All filters are removed successfully and the search results return to their original unfiltered state

---

**Test Case ID:** TC_014

**Title:** Verify the site behaviour when a filter is clicked multiple times

**Summary:** 

Verify that repeatedly clicking the same filter does not cause unexpected behaviour

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. On the search results page, click the same filter multiple times in quick succession
3. Observe the behaviour of the filter and the results

**Expected Result:** 

The filter toggles correctly without causing duplicate filters, page crashes, or unexpected results

**Actual Result:**

The filter toggles correctly without causing duplicate filters, page crashes, or unexpected results

---

**Test Case ID:** TC_015

**Title:** Verify that the price range filter behaves correctly when dragged and returned to its original position

**Summary:** 

Verify that the price range slider handles edge interactions gracefully

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. Locate the price range filter on the search results page
3. Drag the price range slider to a new position
4. Drag the slider back to its original position
5. Observe the results after each adjustment

**Expected Result:** 

The results update correctly with each slider adjustment and the site does not crash or behave unexpectedly

**Actual Result:**

The results update correctly with each slider adjustment and the site does not crash or behave unexpectedly

User receives a message when there are no matching destinations.

---

**Test Case ID:** TC_016

**Title:** Verify that clicking on a property image or name on the search results page redirects the user to the correct property page

**Summary:** 

Verify that property cards on the search results page are clickable and lead to the correct property detail page

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. On the search results page, click on the image of a property
3. Observe the page the user is redirected to
4. Go back and repeat by clicking the property name instead

**Expected Result:** 

Both the image and the name redirect the user to the correct property detail page matching the selected property

**Actual Result:**

Both the image and the name redirect the user to the correct property detail page matching the selected property

---

**Test Case ID:** TC_017

**Title:** Verify that all images on the search results page are visible and properly displayed

**Summary:**

Verify that no property images on the search results page are broken, missing, or misaligned

**Priority:** Low

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. Scroll through the search results page
3. Observe all property images for visibility and alignment

**Expected Result:** 

All property images load correctly and are properly aligned with no broken or missing images

**Actual Result:**

All property images load correctly and are properly aligned with no broken or missing images

---

**Test Case ID:** TC_018

**Title:** Verify that the user can cancel a trip at any point in the booking process

**Summary:** 

Verify that the user can exit or cancel the booking flow at any stage without issues

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. Select a property and proceed into the booking flow
3. At various stages of the booking process, click the back button or navigate away from the page
4. Observe the site behaviour at each stage

**Expected Result:**

The user can exit the booking process at any point and is returned to the previous page or homepage without errors

**Actual Result:**

The user can exit the booking process at any point and is returned to the previous page or homepage without errors

---

## Customization

---

**Test Case ID:** TC_019

**Title:** Verify that the user can change the language of the site

**Summary:** 

Verify that the platform language can be changed and that the UI updates accordingly

**Priority:** High

**Status: Failed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Locate the language selector on the homepage
3. Select a different language from the available options
4. Observe the changes across the page

**Expected Result:** 

The site language updates correctly across all visible content after the selection is made

**Actual Result:**

Some content in the  site are still written in other languages after the language has been changed

---

**Test Case ID:** TC_020

**Title:** Verify that the user can change the currency of the site

**Summary:**

Verify that the platform currency can be changed and that prices update accordingly

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Locate the currency selector on the homepage
3. Select a different currency from the available options
4. Observe the price changes across the page

**Expected Result:** 

All displayed prices update to reflect the selected currency

**Actual Result:**

All displayed prices update to reflect the selected currency

---

**Test Case ID:** TC_021

**Title:** Verify that the user can change the dates and accommodation later in the booking process

**Summary:** 

Verify that the user can go back and modify their selected dates or accommodation after initially proceeding

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. Select a property and proceed into the booking flow
3. Navigate back to the search or property page
4. Change the dates or selected accommodation
5. Proceed forward again

**Expected Result:** 

The updated dates and accommodation are correctly reflected as the user continues through the booking flow

**Actual Result:**

The updated dates and accommodation are correctly reflected as the user continues through the booking flow

---

**Test Case ID:** TC_022

**Title:** Verify the site behaviour after making changes and then navigating back to the previous page

**Summary:** 

Verify that navigating back after making changes does not cause data loss or unexpected behaviour

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. Apply filters or make changes on the search results page
3. Proceed to a property detail page
4. Click the browser back button to return to the search results page
5. Observe whether the previously applied filters and changes are retained

**Expected Result:**

 The user is returned to the search results page with the previously applied filters and changes still intact

**Actual Result:**

 The user is returned to the search results page with the previously applied filters and changes still intact

---

**Test Case ID:** TC_023

**Title:** Verify the site behaviour when the page is refreshed after making changes

**Summary:** 

Verify that refreshing the page after applying filters or changes does not cause errors or data loss

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and perform a valid search
2. Apply filters or make changes on the search results page
3. Refresh the page using Ctrl+R or the browser refresh button
4. Observe the page state after refresh

**Expected Result:** 

The page reloads without errors. Applied filters may or may not persist depending on the site design but no crash or broken layout should occur

**Actual Result:**

The page reloads without errors. Applied filters still persist  

No crash or broken layout occurs

---

**Test Case ID:** TC_024

**Title:** Verify the site behaviour on a slow network connection

**Summary:** 

Verify that the site handles slow network conditions gracefully without crashing or breaking

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Open browser developer tools and throttle the network speed to a slow connection e.g. Slow 3G
2. Navigate to booking.com
3. Perform a search and interact with the search results page
4. Observe loading behaviour, error messages, and overall stability

**Expected Result:** 

The site displays appropriate loading indicators and handles the slow connection gracefully without crashing or showing broken layouts

**Actual Result:**

The site displays appropriate loading indicators and handles the slow connection gracefully without crashing or showing broken layouts

---

# FLIGHTS

---

## Search

---

**Test Case ID:** TC_025

**Title:** Verify that the flight trip type is set to round trip by default

**Summary:**

Verify that when the user navigates to the Flights section, the round trip option is pre-selected by default

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com
2. Click on the Flights section from the navigation header
3. Observe the trip type selection on the flight search form

**Expected Result:** 

The round trip option is selected by default when the Flights section is loaded

**Actual Result:**

The round trip option is selected by default when the Flights section is loaded

---

**Test Case ID:** TC_026

**Title:** Verify that the user can switch between one-way and round trip flight options

**Summary:** 

Verify that the trip type selector allows the user to toggle between one-way and round trip correctly

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Observe the default trip type selection
3. Switch from round trip to one-way
4. Observe the changes in the search form
5. Switch back to round trip
6. Observe the changes again

**Expected Result:**

The search form updates correctly with each trip type selection, 

**Actual Result:**

The search form updates correctly with each trip type selection

The site handles the changes gracefully

---

**Test Case ID:** TC_027

**Title:** Verify that the user can search for a valid flight origin and destination

**Summary:** 

Verify that entering valid origin and destination locations returns relevant flight results

**Priority:** Critical

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Enter a valid departure location e.g. “Lagos”
3. Enter a valid destination location e.g. “London”
4. Select valid departure and return dates
5. Click the Search button

**Expected Result:** 

The user is taken to a search results page displaying available flights matching the entered origin, destination, and dates

**Actual Result:**

The user is taken to a search results page displaying available flights matching the entered origin, destination, and dates

---

**Test Case ID:** TC_028

**Title:** Verify that the user can select valid departure and return dates for a flight

**Summary:** 

Verify that the flight date picker accepts valid departure and return date combinations

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Click on the departure date field
3. Select a valid future departure date
4. Click on the return date field
5. Select a valid return date that is after the departure date

**Expected Result:** 

Both dates are accepted and reflected correctly in the flight search form

**Actual Result:**

Both dates are accepted and reflected correctly in the flight search form

---

**Test Case ID:** TC_029

**Title:** Verify that the user cannot select a past date as a flight departure date

**Summary:** 

Verify that the flight date picker prevents the user from selecting a departure date in the past

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Click on the departure date field
3. Attempt to select a date that is in the past

**Expected Result:**

 Past dates are greyed out and cannot be selected in the flight date picker

**Actual Result:**

 Past dates are greyed out and cannot be selected in the flight date picker

---

**Test Case ID:** TC_030

**Title:** Verify that the user can select the number of passengers for a flight

**Summary:** 

Verify that the passenger count selector allows the user to specify the number of travellers correctly

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Click on the passengers field
3. Increase and decrease the number of adults and children using the provided controls
4. Observe the updated passenger count

**Expected Result:** 

The passenger count updates correctly and is reflected in the flight search query

**Actual Result:**

The passenger count updates correctly and is reflected in the flight search query

---

**Test Case ID:** TC_031

**Title:** Verify that the user can select a flight cabin class

**Summary:** 

Verify that the user can choose from available cabin class options such as economy, business, and first class

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Locate the cabin class selector
3. Click on it and view the available options
4. Select each available class one at a time and observe the selection

**Expected Result:** 

The cabin class selector displays all available options and updates correctly when a selection is made

**Actual Result:**

The cabin class selector displays all available options and updates correctly when a selection is made

---

**Test Case ID:** TC_032

**Title:** Verify that the user can search for a long haul flight

**Summary:** 

Verify that the flight search handles long haul routes and extended date ranges correctly

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Enter a long haul origin and destination e.g. “Lagos” to “Tokyo”
3. Select valid departure and return dates several months apart
4. Click Search

**Expected Result:** 

The search returns relevant long haul flight results(if any) without errors

**Actual Result:**

The search returns relevant long haul flight results without errors

---

**Test Case ID:** TC_033

**Title:** Verify the site behaviour when the user submits an empty flight search

**Summary:** Verify that the flight search form handles an empty submission gracefully

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Leave all search fields empty
3. Click the Search button

**Expected Result:** 

The site displays a validation message prompting the user to fill in the required fields and does not proceed to a results page

**Actual Result:**

User cannot proceed to the next page

The site displays a validation message prompting the user to fill in the required fields 

---

**Test Case ID:** TC_034

**Title:** Verify that the flight search does not accept SQL injection inputs

**Summary:** Verify that the flight search fields are protected against SQL injection attempts

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Enter a common SQL injection string in the origin field e.g. ’ OR ‘1’=’1
3. Click Search
4. Observe the site behaviour

**Expected Result:** 

The site does not execute the injection and either returns no results or displays a validation error without crashing

**Actual Result:**

The site does not execute the injection 

The site displays a validation error without crashing

---

---

**Test Case ID:** TC_035

**Title:** Verify that the flight search results match the entered search query

**Summary:** Verify that all results displayed on the flight search results page correspond to the origin, destination, and dates entered

**Priority:** Critical

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**
1. Navigate to booking.com and go to the Flights section
2. Enter a valid origin, destination, departure date, return date, and passenger count
3. Click Search
4. Review the results on the search results page

**Expected Result:** 

All displayed flight results match the origin, destination, dates, and passenger count that were entered

**Actual Result:**

All displayed flight results match the origin, destination, dates, and passenger count that were entered

---

### CAR RENTALS

---

**Test Case ID:** TC_036

**Title:** Verify that the user can navigate to the Car Rentals section from the navigation header

**Summary:** 

Verify that clicking on the Car Rental tab in the header successfully loads the Car Rentals page

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com
2. Click on the Car Rental tab in the navigation header
3. Observe the page that loads

**Expected Result:** 

The Car Rentals page loads successfully 

**Actual Result:**

The Car Rentals page loads successfully 

---

**Test Case ID:** TC_037

**Title:** Verify that the user can search for a car rental using a valid pick-up location

**Summary:** 

Verify that entering a valid pick-up location in the search bar returns relevant car rental results

**Priority:** Critical

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Car Rental section
2. Click on the Pick-up location field
3. Type a valid location e.g. "Lagos"
4. Select a suggestion from the autocomplete dropdown
5. Set a valid pick-up date and time
6. Set a valid drop-off date and time
7. Click Search

**Expected Result:** 

The user is taken to a search results page displaying available car rentals at the entered pick-up location

**Actual Result:**

The search query is accepted

The user is taken to a search results page displaying available car rentals at the entered pick-up location

---

**Test Case ID:** TC_038

**Title:** Verify that the user can set a pick-up and drop-off date and time for a car rental

**Summary:** 

Verify that the date and time fields for pick-up and drop-off accept valid inputs correctly

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Car Rental section
2. Click on the Pick-up date field and select a valid future date
3. Set a valid pick-up time
4. Click on the Drop-off date field and select a valid date after the pick-up date
5. Set a valid drop-off time
6. Observe that both fields reflect the selected values

**Expected Result:** 

Both the pick-up and drop-off date and time fields accept and display the selected values correctly

**Actual Result:**

Both the pick-up and drop-off date and time fields accept and display the selected values correctly

---

**Test Case ID:** TC_039

**Title:** Verify that the user cannot select a pick-up date in the past

**Summary:** 

Verify that the date picker prevents the user from selecting a past date as the pick-up date

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Car Rental section
2. Click on the Pick-up date field
3. Attempt to select a date that is in the past

**Expected Result:** 

Past dates are greyed out and cannot be selected in the pick-up date field

**Actual Result:**

Past dates are greyed out and cannot be selected in the pick-up date field

---

**Test Case ID:** TC_040

**Title:** Verify that the user can enable the "Drop car off at different location" option

**Summary:** 

Verify that checking the drop-off location checkbox reveals a separate drop-off location input field

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Car Rental section
2. Locate the "Drop car off at different location" checkbox
3. Click the checkbox to enable it
4. Observe the changes in the search form

**Expected Result:** 

A separate drop-off location input field appears and accepts a different location from the pick-up location

**Actual Result:**

A separate drop-off location input field appears and accepts a different location from the pick-up location

---

**Test Case ID:** TC_041

**Title:** Verify that the "Driver aged 30-65?" checkbox is checked by default

**Summary:** 

Verify that the driver age checkbox is pre-selected when the Car Rentals page loads

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Car Rental section
2. Observe the state of the "Driver aged 30-65?" checkbox on page load

**Expected Result:** 

The "Driver aged 30-65?" checkbox is checked by default when the page loads

**Actual Result:**

The "Driver aged 30-65?" checkbox is checked by default when the page loads

---

**Test Case ID:** TC_042

**Title:** Verify that the FAQ section expands and collapses correctly

**Summary:** 

Verify that each FAQ item on the Car Rentals page opens and closes as expected when clicked

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Car Rental section
2. Scroll down to the Frequently Asked Questions section
3. Click on a FAQ item to expand it
4. Observe the content that appears
5. Click the same FAQ item again to collapse it

**Expected Result:** 

The FAQ item expands to reveal the answer when clicked and collapses correctly when clicked again

**Actual Result:**

The FAQ item expands to reveal the answer when clicked and collapses correctly when clicked again

---

**Test Case ID:** TC_043

**Title:** Verify that the popular car rental destinations section displays correctly and is clickable

**Summary:** 

Verify that destination cards in the popular destinations section load with correct details and redirect the user correctly when clicked

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Car Rental section
2. Scroll down to the Popular car rental destinations section
3. Observe that destination cards are displayed with images, names, number of locations, and average prices
4. Click on a destination card

**Expected Result:**

 All destination cards display correctly with relevant details and clicking a card redirects the user to car rental results for that destination

**Actual Result:**

 All destination cards display correctly with relevant details and clicking a card redirects the user to car rental results for that destination

---

### ATTRACTIONS

---

**Test Case ID:** TC_044

**Title:** Verify that the user can navigate to the Attractions section from the navigation header

**Summary:** 

Verify that clicking on the Attractions tab in the header successfully loads the Attractions page

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com
2. Click on the Attractions tab in the navigation header
3. Observe the page that loads

**Expected Result:**

The Attractions page loads successfully with the search bar, top destinations, and explore more destinations sections all visible

**Actual Result:**

The Attractions page loads successfully with the search bar, top destinations, and explore more destinations sections all visible

---

**Test Case ID:** TC_045

**Title:** Verify that the user can search for attractions using a valid destination

**Summary:** 

Verify that entering a valid destination in the search bar returns relevant attraction results

**Priority:** Critical

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Attractions section
2. Click on the Destination field
3. Type a valid destination e.g. "London"
4. Select a suggestion from the autocomplete dropdown
5. Set a valid date
6. Click Search

**Expected Result:** 

The user is taken to a results page displaying available attractions, activities, and experiences at the entered destination

**Actual Result:**

The user is taken to a results page displaying available attractions, activities, and experiences at the entered destination

---

**Test Case ID:** TC_046

**Title:** Verify that the user cannot search for attractions without entering a destination

**Summary:** 

Verify that submitting the search form without a destination displays a validation message

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Attractions section
2. Leave the Destination field empty
3. Click the Search button

**Expected Result:** 

The user is not allowed to proceed

The site displays  attraction suggestions Prompting the user to select one

If the user has searched before, the site suggests the last searched query/ location

**Actual Result:**

The user is not allowed to proceed

The site displays  attraction suggestions Prompting the user to select one

If the user has searched before, the site suggests the last searched query/ location

---

**Test Case ID:** TC_047

**Title:** Verify that the Top Destinations cards load correctly and are clickable

**Summary:** Verify that all destination cards in the Top Destinations section display correctly and redirect the user to the correct page when clicked

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Attractions section
2. Scroll to the Top Destinations section
3. Observe that each card displays a destination image, name, and number of things to do
4. Click on a destination card e.g. "Dubai"

**Expected Result:** 

Each destination card loads correctly with its image and details, and clicking a card redirects the user to the attractions page for that destination

**Actual Result:**

Each destination card loads correctly with its image and details,  

Clicking a card redirects the user to the attractions page for that destination

---

**Test Case ID:** TC_048

**Title:** Verify that the Explore More Destinations region tabs function correctly

**Summary:** 

Verify that clicking on each continent or region tab in the Explore More Destinations section updates the destination grid accordingly

**Priority:** High

**Status:  Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Attractions section
2. Scroll down to the Explore More Destinations section
3. Click on each region tab one at a time e.g. Europe, North America, Asia, Africa, Middle East, Caribbean, South America, Central America
4. Observe the destination grid after each tab is selected

**Expected Result:** 

The destination grid updates correctly to show destinations relevant to the selected region after each tab is clicked

**Actual Result:**

The destination grid updated correctly

The user is redirected to the correct page with content related to what was clicked

---

**Test Case ID:** TC_049

**Title:** Verify that destination cards in the Explore More Destinations section are clickable and redirect correctly

**Summary:** 

Verify that clicking on a destination card in the Explore More Destinations grid takes the user to the correct attractions page for that destination

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Attractions section
2. Scroll down to the Explore More Destinations section
3. Select a region tab
4. Click on any destination card from the grid e.g. "Lagos"
5. Observe the page the user is redirected to

**Expected Result:** 

The user is redirected to an attractions listing page showing Activities, locations and events at the selected destination

**Actual Result:**

The user is redirected to an attractions listing page showing Activities and places at the selected destination

---

### AIRPORT TAXIS

---

---

**Test Case ID:** TC_050

**Title:** Verify that the user can navigate to the Airport Taxis section from the navigation header

**Summary:** 

Verify that clicking on the Airport Taxis tab in the header successfully loads the Airport Taxis page

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com
2. Click on the Airport Taxis tab in the navigation header
3. Observe the page that loads

**Expected Result:** 

The Airport Taxis page loads successfully with the search form, vehicle type options, and FAQ section all visible

**Actual Result:**

The Airport Taxis page loads successfully with the search form, vehicle type options, and FAQ section all visible

---

**Test Case ID:** TC_051

**Title:** Verify that the trip type is set to one-way by default on the Airport Taxis page

**Summary:** 

Verify that when the Airport Taxis page loads, the one-way option is pre-selected by default

**Priority:** Medium

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Airport Taxis section
2. Observe the trip type selection on the search form upon page load

**Expected Result:** 

The one-way option is selected by default when the Airport Taxis page loads

**Actual Result:**

The one-way option is selected by default when the  page loads

---

**Test Case ID:** TC_052

**Title:** Verify that the user can switch between one-way and return trip types

**Summary:**

 Verify that toggling between one-way and return updates the search form correctly

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Airport Taxis section
2. Observe the default one-way selection
3. Click the Return option
4. Observe the changes in the search form
5. Switch back to one-way
6. Observe the changes again

**Expected Result:** 

Selecting Return reveals the return date and time field and switching back to one-way hides it correctly

**Actual Result:**

The system handles the changes gracefully

Selecting Return reveals the return date and time field 

switching back to one-way hides it correctly

---

**Test Case ID:** TC_053

**Title:** Verify that the user can search for an airport taxi using valid pick-up and destination details

**Summary:** 

Verify that entering valid pick-up and destination locations returns available taxi options

**Priority:** Critical

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Airport Taxis section
2. Select the return button, return date and time fields will be added 
3. Enter a valid pick-up location e.g. "Ikoyi, Lagos"
4. Enter a valid destination e.g. "Victoria Island, Lagos"
5. Set a valid date and time
6. Set the number of passengers
7. Click Search

**Expected Result:** 

The user is taken to a results page displaying available taxi options with vehicle details, pricing, and booking options

**Actual Result:**

The user is taken to a results page displaying available taxi options with vehicle details, pricing, and booking options

---

**Test Case ID:** TC_054

**Title:** Verify that the passenger count selector functions correctly

**Summary:** Verify that the passenger count field accepts valid inputs and updates correctly

**Priority:** High

**Status:  Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Airport Taxis section
2. Locate the passenger count selector on the search form
3. Increase the passenger count using the selector
4. Decrease the passenger count back to the original value
5. Observe the changes

**Expected Result:** 

The passenger count updates correctly with each adjustment and reflects the selected value in the search form

**Actual Result:** 

The passenger count updates correctly with each adjustment

Each update reflects the selected value in the search form

---

**Test Case ID:** TC_055

**Title:** Verify that the vehicle type tabs filter results correctly

**Summary:** Verify that selecting different vehicle type tabs on the Airport Taxis page displays the correct vehicle options

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Airport Taxis section
2. Scroll down to the vehicle type tabs section
3. Click on the "1-3 passengers" tab and observe the vehicles displayed
4. Click on the "4-7 passengers" tab and observe the vehicles displayed

**Expected Result:**

 Each tab displays vehicle options relevant to the selected passenger capacity and the displayed cards update correctly with each tab selection

**Actual Result:**

 Each tab displays vehicle options relevant to the selected passenger capacity 

The displayed cards update correctly with each tab selection

---

**Test Case ID:** TC_056

**Title:** Verify that the user can proceed with to next page after clicking on Continue

**Summary:**

Verify that the user can proceed to the contacts page after clicking on the Continue button during the booking process

**Priority:** High

**Status: Passed**

**Environment:** Windows 11

**Browser:** Microsoft Edge

**Steps Taken:**

1. Navigate to booking.com and go to the Airport Taxis section
2. Enter a valid pick-up location, destination, date, time, and passenger count
3. Click Search
4. Select an available taxi option from the results page
5. Click the Continue  button

**Expected Result:** 

The user is redirected to a new page where they are required to provide their contact information

**Actual Result:**

The user is redirected to a new page where they are to provide their contact information 

---
