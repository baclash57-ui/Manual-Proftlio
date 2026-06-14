**Project:** Booking.com QA Review

**Prepared by:** Japhet Obinna Prosper

**Test Type:** Manual Functional Testing

**Environment:** Live Production Site (booking.com)

**Scope:** Guest User Flow Only (Not Logged In)

---

## 1. Objective

The objective of this test plan is to validate the core functional behaviour of Booking.com as experienced by a guest user. Testing will focus on ensuring that all in-scope user flows work as expected on the live site, without deviating from the defined scope. Payment flows are explicitly excluded from this test cycle.

---

## 2. Scope

### In Scope

- Homepage Search & Recommendations
- Flights
- Car Rentals
- Attractions
- Airport Taxis
- Reviews (read only)
- Help & Support (FAQs)
- Languages & Themes

### Out of Scope

- Payment and checkout completion
- Sign In / Register flows
- Submitting reviews
- Customer support (live chat or direct contact)
- List your Property
- Footer links
- External sites that is sites without  the domain: Bookings.com
- Associates, affiliates, Privacy Policies, Terms of Use
- Minor UI issues that do not affect user flow
- Discounts tied to signing in or registering

---

## 3. Test Approach

Since this is a **live production site**, testing must be conducted with care. No test transactions will be completed and no bookings will be finalised. Testing will navigate up to but not including the payment confirmation step.

All testing will be **manual and functional**, validating that each feature behaves correctly from the perspective of a guest user. The Tester will follow the defined user flows, verify that UI elements respond as expected, and document any deviations or defects observed.

---

## 4. Assumptions & Preconditions

- Tester must be logged out of any existing Booking.com account before starting
- Testing will be conducted as a guest (unauthenticated) user at all times
- A stable internet connection must be available throughout the test session
- Tests will be carried out on a modern browser (Chrome, Firefox, or Edge — latest stable versions)
- The live site is accessible and not under maintenance at the time of testing
- No bookings will be completed or payments submitted during testing
- Test data used (e.g. destinations, dates) must be realistic and valid to trigger proper results

---

## 5. Entry Criteria

The following conditions must be met before testing can begin:

- The test plan has been reviewed and approved
- All in-scope areas have been clearly defined and agreed upon
- Testers have been briefed on the scope, constraints, and preconditions
- The live site (booking.com) is accessible and functioning at a basic level
- Test cases have been documented and are ready for execution
- Testers are confirmed to be logged out of any Booking.com account
- Test environment details (browsers, devices) have been confirmed

---

## 6. Exit Criteria

Testing will be considered complete when the following conditions are met:

- All test cases across in-scope areas have been executed at least once
- All critical and high severity defects have been logged with sufficient detail
- No outstanding critical bugs are blocking core user flows without being documented
- A test summary report has been prepared detailing pass/fail results and defect counts
- All defects have been triaged and assigned a severity level
- Sign-off has been obtained from the QA lead

---

## 7. Test Areas & High-Level Test Scenarios

### 7.1 Homepage Search & Recommendations

- Verify that the homepage loads correctly with property recommendations visible
- Verify that the search bar accepts a valid destination and returns relevant results
- Verify that the date picker allows valid check-in and check-out date selection
- Verify that the guest and room count selector functions correctly
- Verify that clicking a recommended property navigates to the correct listing
- Verify that trending destination cards are clickable and load relevant search results

### 7.2 Flights

- Verify that the user can navigate to the Flights section from the homepage
- Verify that the user can select one-way or round trip flight options
- Verify that the user can enter a valid origin and destination and initiate a search
- Verify that flight results are displayed with relevant details (airline, price, duration)
- Verify that filters (price, duration, airline, baggage) update results correctly
- Verify that the user can select a flight and proceed to the passenger details step without completing payment

### 7.3 Car Rentals

- Verify that the user can navigate to the Car Rentals section
- Verify that the user can search for a car rental by entering a valid pickup location and date
- Verify that available car options are returned with details (car type, price, provider)
- Verify that the user can apply filters and sort options on the results page
- Verify that the user can select a car and proceed to the booking details step without completing payment

### 7.4 Attractions

- Verify that the user can navigate to the Attractions section
- Verify that the user can search for attractions at a valid destination
- Verify that attraction listings load with relevant details (name, description, price, availability)
- Verify that the user can select an attraction and view its full detail page
- Verify that the user can proceed to the booking step without completing payment

### 7.5 Airport Taxis

- Verify that the user can navigate to the Airport Taxis section
- Verify that the user can enter valid pickup and drop-off location details
- Verify that available taxi options are returned with vehicle type and pricing details
- Verify that the user can select a taxi option and proceed to the next step without completing payment

### 7.6 Reviews

- Verify that guest reviews are visible on property and attraction listing pages
- Verify that review details (rating score, reviewer name, review text, date) are displayed correctly
- Verify that the user can scroll through or paginate multiple reviews on a listing

### 7.7 Help & Support (FAQs)

- Verify that the Help/FAQ section is accessible from the homepage
- Verify that the user can search for a topic and receive relevant FAQ results
- Verify that FAQ articles open and display complete, readable content

### 7.8 Languages & Themes

- Verify that the user can change the platform display language
- Verify that the UI content updates correctly after a language change
- Verify that the user can switch display themes where available and that the change is reflected across the page

---

## 8. Defect Management

All defects identified during testing will be logged with the following information:

- **Defect ID** — Unique identifier
- **Test Area** — The section of the site where the defect was found
- **Description** — Clear summary of the issue observed
- **Steps to Reproduce** — Step-by-step instructions to replicate the defect
- **Expected Result** — What should have happened
- **Actual Result** — What actually happened
- **Severity** — Critical / High / Medium / Low
- **Screenshot/Evidence** — Attached where applicable

### Severity Definitions

- **Critical** — Core user flow is completely broken (e.g. search returns no results at all, page fails to load)
- **High** — Major feature is not functioning correctly but a workaround may exist
- **Medium** — Feature works but behaves unexpectedly in certain conditions
- **Low** — Minor issue with no significant impact on the user flow

---

## 9. Risks & Mitigations

| Risk | Impact | Mitigation |
| --- | --- | --- |
| Live site may undergo updates or changes during testing | Test results may be inconsistent | Document the date and time of each test session |
| Pricing and availability data changes frequently | Results may vary between sessions | Use realistic but non-specific test data and note variability |
| Network instability on tester's end | False failures may be logged | Confirm stable connection before each session; retest before logging |
| Site may detect and rate-limit repeated searches | Searches may be blocked or skewed | Space out test executions and avoid repetitive identical searches |
| Regional content differences may affect results | Some features may appear/behave differently by location.                Testing conducted from Anambra, Nigeria. Regional content differences may apply. | Note tester location in the test report |

### Note:

**Testing conducted from Anambra, Nigeria. Regional content differences may apply**.
**Testing wwas conducted during febuary bugs might not be reproducible when tested due to updates in the version of the site**.


---

## 10. Test Deliverables

- Test Plan (this document)
- Test Cases per in-scope area
- Test Execution Report (pass/fail per test case)
- Defect Log with severity ratings
- Test Summary Report upon completion

---
