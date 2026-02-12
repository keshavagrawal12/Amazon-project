# Javascript Amazon Project

This is an e-commerce web application that mimics the core functionality of Amazon. It includes product listing, a shopping cart, checkout process, and order tracking.

## Features

- **Product Listing:** Browse products on the main page (`amazon.html`).
- **Shopping Cart:** Add items to the cart and view them (`checkout.html`).
- **Checkout:** Proceed to checkout, select delivery options, and place orders.
- **Orders:** View past orders (`orders.html`).
- **Tracking:** Track the status of orders (`tracking.html`).

## Installation & Usage

To run this project, simply open the HTML files in your web browser. It is preferred to use a local server (like Live Server in VS Code) for a better experience.

<<<<<<< HEAD
1.  **Clone the repository:**
    ```bash
<<<<<<< HEAD
    git clone https://github.com/keshavagrawal12/Amazon-project.git
=======
    git clone https://github.com/yourusername/javascript-amazon-project.git
>>>>>>> 4f241b7 (Update README to GitHub detailed version)
    cd javascript-amazon-project
    ```

2.  **Run the application:**
    - **Recommended:** Use a VS Code extension like **Live Server**. Right-click `amazon.html` and select "Open with Live Server".
    - **Alternative:** Simply open `amazon.html` in your preferred web browser.

3.  **Navigate:** Use the header links to switch between the product page, cart, orders, and tracking pages.
=======
1.  Clone or download the repository.
2.  Open `amazon.html` to start browsing products.
3.  Navigate through the app using the links provided in the interface.
>>>>>>> e9a27b2 (Save local changes before pulling)

## Testing

This project includes both manual and automated tests to ensure functionality.

### 1. Manual Tests
A simple manual test script is available for checking currency formatting.
- **File:** `tests/tests.html`
- **How to run:** Open `tests/tests.html` in your browser and check the **Console** (F12 > Console tab) to see "passed" or "failed" messages.

### 2. Jasmine Tests Framework
The project uses the Jasmine testing framework for more robust unit and integration testing.
- **File:** `tests-jasmine/SpecRunner.html`
- **How to run:** Open `tests-jasmine/SpecRunner.html` in your browser. The test results will be displayed on the page.

#### About the tests run
The following test suites are included:
- **Money Utils (`moneyTest.js`):** Verifies that the currency formatting utility correctly handles cents, zero values, and rounding.
- **Cart Data (`cartTest.js`):** Tests the `addToCart` function, ensuring products are correctly added to the cart array and LocalStorage is updated.
- **Order Summary (`orderSummaryTest.js`):** Tests the checkout page rendering (`renderOrderSummary`), verifying that the correct number of cart items are displayed in the DOM.

## Limitations

- **Time Display:** The time is currently not showing in the cart.
- **Mock Backend:** The project uses a local `backend/products.json` and does not connect to a live payment gateway or database.
