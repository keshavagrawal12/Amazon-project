# Javascript Amazon Clone

![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E)

A lightweight e-commerce web application that replicates the core functionality of Amazon. This project demonstrates vanilla JavaScript DOM manipulation, modular code structure, and automated testing with Jasmine.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation & Usage](#installation--usage)
- [Testing](#testing)
- [Project Structure](#project-structure)
- [Limitations](#limitations)
- [License](#license)

## Features

- **Product Listing:** Dynamic grid of products fetched from a local data source (`amazon.html`).
- **Shopping Cart:** Add items to cart with quantity updates and persistence using `localStorage`.
- **Checkout Process:** Calculate totals, shipping costs, and tax (`checkout.html`).
- **Order Management:** Place orders and view order history (`orders.html`).
- **Tracking:** Simulate order tracking functionality (`tracking.html`).

## Technologies Used

- **Frontend:** HTML5, CSS3, Vanilla JavaScript (ES6+ Modules)
- **Testing:** Jasmine Framework
- **Storage:** LocalStorage (for cart persistence)

## Installation & Usage

No complex build steps are required. You can run this project directly in the browser, though using a local development server is recommended for the best experience.

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

## Testing

This project employs a comprehensive testing strategy using both manual verification and the Jasmine testing framework.

### Automated Tests (Jasmine)

The project includes a suite of unit and integration tests to verify core logic:

- **Money Utilities (`moneyTest.js`):** Validates currency formatting logic (handling cents, rounding, zero values).
- **Cart Logic (`cartTest.js`):** Tests adding products to the cart, updating local storage correctly.
- **Order Summary (`orderSummaryTest.js`):** Integration test for the checkout page rendering, ensuring the DOM updates correctly based on cart contents.

**To run the tests:**
1. Open `tests-jasmine/SpecRunner.html` in your browser.
2. View the test results on the page (Green for pass, Red for fail).

### Manual Tests

A simple manual test script is also provided in `tests/tests.html`. Open this file and check the browser Console (F12) for "passed/failed" logs.

## Project Structure

```text
/
├── amazon.html         # Main product listing page
├── checkout.html       # Cart and checkout page
├── orders.html         # Order history page
├── tracking.html       # Order tracking page
├── backend/            # Mock backend data
├── data/               # Data modules (cart, products, delivery options)
├── scripts/            # Application logic
│   ├── checkout/       # Checkout page scripts
│   └── utils/          # Utility functions (money formatting)
├── styles/             # CSS stylesheets
├── tests/              # Manual test scripts
└── tests-jasmine/      # Jasmine test suite
```

## Limitations

- **Time Display:** The current time is not displayed in the cart header.
- **Mock Backend:** The project uses a static `backend/products.json` file. It does not connect to a real database or payment gateway.
- **Payment Processing:** No actual payments are processed; the "Place Order" button simulates a successful transaction.

## License

This project is licensed under the MIT License - see the `tests-jasmine/MIT.LICENSE` file for details.
