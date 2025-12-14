# Milestone 4: Booking Detail Page Implementation

**Project:** ALX Listing App
**Milestone:** 04
**Repository:** `alx-listing-app-03`

## 📋 Overview

In this milestone, we implemented a fully functional **Booking Detail Page** for the listing application. This page mirrors real-world travel platforms (like Airbnb or Booking.com) by allowing users to review property details, enter contact and billing information, and view a dynamic price breakdown before confirming their reservation.

The project emphasizes component-based architecture using **Next.js**, **TypeScript**, and responsive styling with **Tailwind CSS**.

## 🎯 Learning Objectives

* **Component-Based Architecture:** Splitting the UI into reusable components (`BookingForm`, `OrderSummary`, `CancellationPolicy`).
* **Responsive Design:** Using Tailwind CSS grid and utility classes to ensure the layout works on mobile and desktop.
* **Form Handling:** Structuring complex forms with grouped inputs for contact and payment details.
* **Dynamic Data:** Passing props to child components to calculate totals and display specific property info.

## 🛠️ Tech Stack

* **Framework:** Next.js
* **Language:** TypeScript
* **Styling:** Tailwind CSS
* **Library:** React

## 📂 Project Structure

The folder structure for this milestone is organized as follows:

```text
alx-listing-app-03/
├── components/
│   └── booking/
│       ├── BookingForm.tsx         # Collects user contact & payment info
│       ├── OrderSummary.tsx        # Displays price breakdown & stay details
│       └── CancellationPolicy.tsx  # Shows rules and refund policies
├── pages/
│   └── booking/
│       └── index.tsx               # Main page assembling all components
└── README.md


## 🚀 Features Implemented 
#1. Booking Form (BookingForm.tsx)
A comprehensive form that collects user data. It uses Tailwind's grid-cols-2 to create a responsive layout for:

Contact Info: First Name, Last Name, Email, Phone Number.

Payment Details: Card Number, Expiration Date, CVV.

Billing Address: Street, City, State, Zip Code, Country.

#2. Order Summary (OrderSummary.tsx)
A dynamic sidebar component that displays:

Property name, image, and review score.

Stay details (Start Date, Total Nights).

Price Breakdown: Automatically calculates Booking Fee + Subtotal to display the Grand Total.

#3. Cancellation Policy & Ground Rules (CancellationPolicy.tsx)
A static information section that outlines:

Cancellation Policy: Refund terms based on dates.

Ground Rules: House rules for guests (e.g., "Follow the house rules").

💻 How to Run
Duplicate/Clone the repository:

Bash

git clone <repository-url>
Navigate to the project folder:

Bash

cd alx-listing-app-03
Install dependencies:

Bash

npm install
Run the development server:

Bash

npm run dev
View the application: Open http://localhost:3000/booking in your browser.

