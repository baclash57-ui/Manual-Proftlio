# Booking.com — Final Test Summary Report

**Project:** Booking.com QA Review
**Prepared by:** Obinna Japhet
**Test Type:** Manual Functional Testing & Exploratory Testing
**Environment:** Windows 11
**Browser:** Microsoft Edge
**Tester Location:** Nigeria
**Date:** February 27, 2026

---

## 1. Objective

The objective of this report is to summarize the outcome of all testing activities conducted on the Booking.com live site. This includes manual functional test case execution and exploratory testing, covering all in-scope areas as defined in the Test Plan. Payment flows were explicitly excluded from all testing activities.

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
- Customer support
- List your Property
- Footer links
- Associates, affiliates, Privacy Policies, Terms of Use
- Minor UI issues that do not affect user flow
- Discounts tied to signing in or registering

---

## 3. Test Case Execution Summary

### 3.1 Overall Results

| Metric | Count |
| --- | --- |
| Total Test Cases Executed | 56 |
| Passed | 55 |
| Failed | 1 |
| Blocked | 0 |
| Pass Rate | 98.2% |

### 3.2 Results by Section

| Section | Total | Passed | Failed |
| --- | --- | --- | --- |
| Homepage — General Page Behaviour | 5 | 5 | 0 |
| Homepage — Search & Filter | 13 | 13 | 0 |
| Homepage — Customization | 6 | 5 | 1 |
| Flights | 11 | 11 | 0 |
| Car Rentals | 8 | 8 | 0 |
| Attractions | 6 | 6 | 0 |
| Airport Taxis | 7 | 7 | 0 |
| **Total** | **56** | **55** | **1** |

### 3.3 Failed Test Case

| TC ID | Title | Section | Priority | Severity |
| --- | --- | --- | --- | --- |
| TC_019 | Verify that the user can change the language of the site | Homepage — Customization | High | Medium |

**Details:Expected Result:** The site language updates correctly across all visible content after the selection is made
**Actual Result:** Some content on the site continued to display in other languages after the language was changed

---

## 4. Observations & Notable Findings from Test Case Execution

**TC_010 — Homepage Search**
When an invalid destination is entered the site does not return an empty results page. Instead it displays a message and provides alternative destination suggestions, which is a positive UX behaviour.

**TC_015 — Price Range Filter**
When the price range slider is dragged to a position where no properties match, the site displays a message informing the user that there are no matching results. This is graceful error handling and a positive finding.

**TC_023 — Page Refresh After Changes**
Applied filters persist after a page refresh, preventing users from losing their search preferences. This is a positive UX behaviour.

**TC_047 — Attractions Empty Search**
When the search field is left empty, the site displays attraction suggestions and if the user has previously searched, it surfaces the last searched location. This is an enhanced UX behaviour that goes beyond a basic validation message.

---

## 5. Exploratory Testing Summary

### 5.1 Overall Bug Summary

| Metric | Count |
| --- | --- |
| Total Bugs Found | 3 |
| Functional Bugs | 3 |
| Critical | 0 |
| High | 0 |
| Medium | 3 |
| Low | 0 |

### 5.2 Bug List

| Bug ID | Title | Type | Severity | Status | Related TC |
| --- | --- | --- | --- | --- | --- |
| BG_LN_001 | Several sections in the Attractions page show content in different languages after the user changes language | Functional | Medium | Open | TC_019 |
| BG_CR_001 | Some sections of the Attractions destination listing page do not display prices in the user's local currency on page load | Functional | Medium | Open | None |
| BG_CR_002 | User cannot change their currency back to their local currency after switching it | Functional | Medium | Open | None |

### 5.3 Bug Breakdown by Category

| Category | Count |
| --- | --- |
| Language (BG_LN) | 1 |
| Currency (BG_CR) | 2 |

### 5.4 Bug Summaries

**BG_LN_001 — Language inconsistency on Attractions page**
After changing the site language, several sections on the Attractions page continue to display content in other languages. This finding is consistent with the TC_019 failure identified during test case execution and confirms the issue is specifically present on the Attractions page.

**BG_CR_001 — Currency inconsistency on Attractions destination listing page**
When the site is loaded with the user's local currency as default and no currency changes have been made, several sections on the Attractions destination listing page display prices in a different currency. This was a new finding from exploratory testing not covered during test case execution.

**BG_CR_002 — User cannot change currency back to local currency**
After switching the currency on the site, the user is unable to change it back to their local currency. The currency selector does not display the user's local currency after a currency change has been made. This applies to users whose local currency is not internationally traded and was a new finding from exploratory testing.

---

## 6. Test Case Impact Analysis

| Bug ID | Related TC | TC Title | TC Status | Impact |
| --- | --- | --- | --- | --- |
| BG_LN_001 | TC_019 | Verify that the user can change the language of the site | Failed | Bug confirmed and consistent with TC_019 failure |
| BG_CR_001 | None | N/A | N/A | New exploratory finding — not covered in test case execution |
| BG_CR_002 | None | N/A | N/A | New exploratory finding — not covered in test case execution |

---

## 7. Recommendations

- **BG_LN_001** — The development team should investigate why language changes are not being applied consistently across all sections of the Attractions page and ensure all content updates correctly when the language is changed
- **BG_CR_001** — The currency display logic on the Attractions destination listing page should be reviewed to ensure all sections reflect the user's local currency correctly on page load
- **BG_CR_002** — The currency selector should be investigated to ensure users can switch back to their local currency at any point regardless of whether their currency is internationally traded
- Two new test cases should be added to the test case suite to cover the currency-related bugs found during exploratory testing to ensure they are captured in future test cycles

---

## 8. Test Coverage Summary

| Area | Coverage |
| --- | --- |
| Homepage navigation and layout | ✅ Covered |
| Search functionality | ✅ Covered |
| Date picker validation | ✅ Covered |
| Filter functionality | ✅ Covered |
| Customization — language and currency | ✅ Covered |
| Flights search and filtering | ✅ Covered |
| Security — SQL injection | ✅ Covered |
| Car Rentals search and options | ✅ Covered |
| Attractions search and navigation | ✅ Covered |
| Airport Taxis search and booking flow | ✅ Covered |
| Payment completion | ❌ Out of Scope |

---

## 9. Conclusion

All planned test case execution and exploratory testing activities for the Booking.com live site have been completed as of February 27, 2026. A total of **56 test cases were executed** with a **pass rate of 98.2%**, and **3 medium severity bugs** were identified during exploratory testing. All bugs are related to localisation — specifically language and currency consistency across the site. No critical or high severity defects were identified and no core user flows were found to be broken.

The two new currency-related bugs identified during exploratory testing were not covered during the test case execution cycle and are recommended for inclusion in future test cases.

---

## 10. Overall Project Status

| Activity | Status |
| --- | --- |
| Test Case Execution | ✅ Complete — 98.2% pass rate, 1 failed test case |
| Exploratory Testing | ✅ Complete — 3 medium severity bugs logged |
| Open Defects | 3 open defects pending investigation |
| **Overall Project Status** | **✅ PASS — with 3 open defects to be investigated** |

---
