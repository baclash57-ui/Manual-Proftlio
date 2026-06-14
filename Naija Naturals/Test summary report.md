# NN Hair & Beauty – Test Summary Report

---

## Report Details

| Field | Details |
| --- | --- |
| Project | NN Hair & Beauty – naijanaturals.com |
| Prepared By | Obinna Japhet |
| Test Date | February 18, 2026 |
| Environment | Windows 11 |
| Browser | Microsoft Edge (Latest Stable) |
| Test Cycle | Cycle 1 – Functional & UI Testing |
| Report Status | Final |

---

## Objective

The objective of this test cycle was to validate the core user-facing functionality of the NN Hair & Beauty website (naijanaturals.com) across six key areas — Homepage, Search & Filter, Product Description Page, Cart Section, Product Listing & Category Pages, and Checkout (Pre-Payment). Testing was conducted on a Windows 11 desktop machine using Microsoft Edge and covered the end-to-end user journey from the homepage through to the checkout entry point. Payment processing was explicitly excluded from this test cycle.

---

## Scope Summary

| Area | In Scope | Out of Scope |
| --- | --- | --- |
| Homepage | ✅ |  |
| Search & Filter | ✅ |  |
| Product Description Page (PDP) | ✅ |  |
| Cart Section | ✅ |  |
| Product Listing & Category Pages | ✅ |  |
| Checkout (Pre-Payment) | ✅ |  |
| Payment Processing |  | ✅ |
| Login & Registration |  | ✅ |
| Footer Links |  | ✅ |
| Social Media Handles |  | ✅ |
| UK Store |  | ✅ |
| Newsletter Section |  | ✅ |
| Contact Us |  | ✅ |
| Order Tracking |  | ✅ |
| Wishlist / Save for Later |  | ✅ |
| Mobile & Tablet Responsiveness |  | ✅ |
| Cross-Browser Testing |  | ✅ |
| Performance & Load Testing |  | ✅ |
| Accessibility (WCAG) Testing |  | ✅ |

## Test Pass Rate

| Metric | Result |
| --- | --- |
| Total Test Cases Executed | 23 |
| Total Passed | 22 |
| Total Failed | 1 |
| Overall Pass Rate | 95.6% |
| Exit Criteria Threshold | 90% |
| Exit Criteria Met | ✅ Met (With Quality Caveats) |

> **Note:** While the numerical pass rate of 95.6% clears the 90% exit criteria threshold, significant functional defects were discovered during testing (including a High-priority search defect and a routing bug). Because these issues directly impact the user experience, final sign-off should be withheld until critical fixes are applied.

---

## Defects Summary

| Bug ID | Title | Area | Priority | Status |
| --- | --- | --- | --- | --- |
| BG-NN_001 | Nationwide Fast Delivery button redirects user to the FAQ page | Homepage | Medium | Open |
| BG-NN_002 | Search Results Page returns unrelated items | Search & Filter | High | Open |

---

## Defects by Priority

| Priority | Count |
| --- | --- |
| High | 1 |
| Medium | 1 |
| Low | 0 |
| **Total** | **2** |

---

## Test Results by Area

**Homepage**
A total of 6 test cases were executed for the homepage. All 6 passed successfully from a pure text execution standpoint (including graceful performance degradation on a slow network link). However, exploratory logging captured defect **BG-NN_001**, where the "Nationwide Fast Delivery" button below the logo points to the FAQ page instead of delivery details.

**Search & Filter**
A total of 8 test cases were executed. 7 passed and 1 failed. The explicit failure was **TC_SF_004** (*Adjusting price range filter updates results correctly*), which tied into the broader functional defect **BG-NN_002**, where searching for explicit terms like "Hair Dye" introduces completely unrelated products to the user grid.

**Product Description Page (PDP)**
A total of 4 test cases were executed for the PDP. All 4 passed successfully. Variant selectors, image clicking, back navigation, and the core "Add to Cart" button actions all performed exactly to specification.

**Cart Section**
A total of 5 test cases were executed for the Cart section. All 5 passed successfully. Subtotal calculations, quantity scaling (increasing/decreasing items), item removals, and session retention when navigating away from the cart behaved correctly.

---

## Risk Assessment

The primary operational risk to this release is **BG-NN_002** (Search Results Page returning unrelated items). Because search is the primary driver for e-commerce conversions, inaccurate or messy results heavily break user trust and degrade customer retention.

**BG-NN_001** poses a minor navigation risk, routing users searching for direct shipping policies to a general FAQ page.

---

## Recommendations

* **Hold the release deployment** until high-priority bug **BG-NN_002** is patched and verified.
* Resolve the button routing on the homepage (**BG-NN_001**) to point to the correct delivery information asset.
* Perform a targeted regression sweep across the Search & Filter modules once developer fixes are applied.

---

## Entry & Exit Criteria Status

| Criteria | Status |
| --- | --- |
| 100% of test cases executed | ✅ Met |
| All P1 (Critical) defects resolved | ✅ Met (None identified) |
| All P2 (High) defects resolved | ❌ Not Met (BG-NN_002 remains open) |
| 90% minimum pass rate achieved | ✅ Met (95.6% achieved) |
| Test summary report produced | ✅ Met |
| Stakeholder sign-off obtained | ⏳ Pending |

---

## Overall Verdict

> ❌ **NOT READY FOR RELEASE**
> The testing cycle is complete and the raw pass rate meets requirements, but the exit criteria are not fully satisfied due to the open High-Priority defect (**BG-NN_002**). Release sign-off should be granted only after search integrity is restored.

---

## Sign-Off

| Field | Details |
| --- | --- |
| Prepared By | Obinna Japhet|
| Reviewed By |  |
| Approved By |  |
| Date | February 18, 2026 |
| Report Version | 1.0 |

---

---

