<img width="1917" height="1012" alt="image" src="https://github.com/user-attachments/assets/acb6764b-cbe8-46a8-aced-5b0c5cf21be1" />


# Project Overview

### Link:

bookings.com 

---

## Platform Description

Booking.com is a leading online travel and accommodation platform that allows users to search and book hotels, homes, and other properties worldwide. In addition to accommodations, the platform offers flight booking, car rentals, airport taxis, and attraction tickets — making it a comprehensive travel planning tool for vacations, business trips, relocation, and more. Booking.com also provides answers to travel-related questions and access to millions of traveller reviews.

---

## Core User Flows

### 1. Homepage

- Verify that recommended properties are displayed on the homepage upon arrival
- Verify that the user can search for a destination using the search bar
- Verify that the user can set check-in and check-out dates using the date picker
- Verify that the user can specify the number of guests and rooms before searching
- Verify that trending destinations and property category sections are visible and clickable

### 2. Explore

- Verify that the user can browse and interact with destination locations on the map
- Verify that the user can access the Help/FAQ section to get answers to travel-related questions

### 3. Flights

- Verify that the user can select a flight type (one-way or round trip)
- Verify that the user can enter different origin and destination combinations when searching for flights
- Verify that the user can search for flights on behalf of another person
- Verify that the user can filter flight results by airline, baggage allowance, price, and duration
- Verify that flight results update correctly when filters are applied or changed

### 4. Lodgings

- Verify that the user can search for hotels, apartments, resorts, and vacation rentals
- Verify that the user can apply filters such as price range, property type, and guest rating
- Verify that the user can view property details including photos, amenities, and location
- Verify that the user can read guest reviews on a property listing
- Verify that the user can select a room type and proceed to booking

### 5. Payment

- Verify that the user can select a payment method (e.g. credit/debit card)
- Verify that the user can enter billing details on the payment page
- Verify that a booking summary is displayed before final payment submission
- Verify that the user receives a booking confirmation after successful payment

---

## Assumptions / Preconditions

- Testing will be conducted as a guest user (not logged in)
- If a tester has an existing Booking.com account, they must log out before beginning testing to avoid account-based personalisation or suspicious activity detection by the platform
- Reviews testing covers the ability to read and browse existing reviews only — submitting reviews is out of scope

---

## In-Scope Areas

### 1. Homepage Search & Recommendations

- Verify that the search bar is functional and returns relevant results based on the destination entered
- Verify that the date picker allows valid check-in and check-out date selection
- Verify that homepage property recommendations load correctly and are clickable

### 2. Flights

- Verify that the user can search for available flights using valid origin and destination inputs
- Verify that one-way and round trip options function correctly
- Verify that flight filters (airline, price, duration, baggage) return accurate, updated results

### 3. Car Rentals

- Verify that the user can search for available car rentals by location and date
- Verify that car rental options are displayed with relevant details (price, car type, provider)
- Verify that the user can select a car rental and proceed to the booking step

### 4. Attractions

- Verify that the user can browse and search for attractions at a given destination
- Verify that attraction listings display relevant details such as description, price, and availability
- Verify that the user can select an attraction and proceed to booking

### 5. Airport Taxis

- Verify that the user can search for airport taxi services by entering pickup and drop-off locations
- Verify that available taxi options are displayed with pricing and vehicle details
- Verify that the user can select a taxi option and proceed to the booking step

### 6. Reviews

- Verify that guest reviews are visible on property and attraction listing pages
- Verify that reviews display relevant information such as rating, reviewer name, and review text
- Verify that the user can scroll through or paginate multiple reviews

### 7. Help & Support (FAQs)

- Verify that the Help/FAQ section is accessible from the homepage
- Verify that the user can search for a topic within the FAQ section and receive relevant results
- Verify that FAQ articles load correctly and display complete, readable content

### 8. Languages & Themes

- Verify that the user can change the platform language and that the UI updates accordingly
- Verify that the user can switch between display themes (e.g. light/dark) where available

---

## Out-of-Scope Areas

- Footer links
- Sign In / Register flows
- Customer support (live chat or direct contact)
- Associates and affiliates
- Privacy Policies
- Terms of Use
- List your Property (for hosts and property owners)
- Minor UI issues that do not affect user flow (e.g. image misalignment, low image quality)
- Discounts or features tied to signing in or registering
- Settings and legal pages
- Submitting reviews
- External links ie  any link unelated to the domain : Bookings.com/
- Payment Section
