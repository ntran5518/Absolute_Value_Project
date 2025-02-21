# Absolute Value - eCommerce Mobile Application

## Project Overview

**Absolute Value** is a mobile eCommerce application designed to provide a seamless shopping experience. Users can browse a product catalog, view product details, add items to their cart, and complete purchases. The application is built using **Dart** and **Flutter** for the front-end, with **Android Studio** as the primary emulator and **VS Code** as the development environment.

Our goal is to create a user-friendly and visually appealing shopping experience, leveraging Flutter's widget system to build an interactive and modern UI.

## Features

### Screens

1. **Welcome Screen**
   - Displays the app logo, introduction, and an emoji-changing button for user enjoyment.

2. **Catalogue Screen**
   - List of available products with:
     - ID, Name, Description, Inventory Quantity
     - "Add to Cart" button (decrements stock count upon selection)
     - "Details" button to navigate to the product details page
   - If inventory reaches zero, the "Add to Cart" button is disabled

3. **Product Details Screen**
   - Displays product-specific details, including:
     - Name, Image, Price, and Stock Quantity

4. **Shopping Cart Screen**
   - Lists items added to the cart
   - Displays:
     - Item ID, Name, Price, and Quantity
   - "Go to Checkout" button to navigate to the next screen
   - If the cart is empty, an empty cart message is shown

5. **Customer Information Screen**
   - Form for user input, including:
     - Name (required field)
     - Email (required, validated format)
     - Store membership status (switch toggle)
     - Email receipt preference (checkbox)
   - "Submit" button to validate and process input before proceeding to checkout

6. **Success (Receipt) Screen**
   - Displays a success message with:
     - Order receipt including product quantities, cost, tax, and total
     - If the user is a store member, a 5% discount is applied
   - "Back to Home" button to return to the Welcome Screen

## Navigation

The app employs a **Tab Navigation Bar** and **Stack Navigation** for smooth transitions between screens:

- **Tab Navigation:** Main screens (Welcome, Catalogue, Shopping Cart)
- **Stack Navigation:**
  - Catalogue → Shopping Cart
  - Catalogue → Product Details
  - Shopping Cart → Customer Information
  - Customer Information → Success (Receipt)
  - Success → Welcome

## Styles & Formatting

- **Consistent Color Scheme:** A unified color theme throughout the app
- **Widgets Used:**
  - Layout widgets: Container, Row, Column, Center
  - UI elements: TextStyle, Image, Icon

## Data Persistence

- User purchase data is saved using **Shared Preferences**, ensuring persistent shopping cart details.

## Development Environment

- **Programming Language:** Dart
- **Framework:** Flutter
- **Code Editor:** VS Code
- **Emulator:** Android Studio (Koala version)

## Installation & Running the Project

### Prerequisites

Ensure you have the following installed:

- [Flutter SDK](https://flutter.dev/docs/get-started/install)
- [Dart](https://dart.dev/get-dart)
- [Android Studio](https://developer.android.com/studio)
- [VS Code](https://code.visualstudio.com/)

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/ntran5518/Absolute_Value_Project.git
   cd Absolute_Value_Project
   ```
2. Install dependencies:
   ```bash
   flutter pub get
   ```
3. Run the application:
   ```bash
   flutter run
   ```

## Work Assignments

| Group Member    | Responsibilities                                                                                             |
| --------------- | ------------------------------------------------------------------------------------------------------------ |
| **Nini Tran**   | Screens: Shopping Cart, Customer Information  Navigation: Tab Navigation, Stack Navigation  Data Persistence, Welcome, Success (Receipt), Catalogue, Product Details  Navigation: Stack Navigation |

## Contribution Guidelines

1. Fork the repository
2. Create a new branch for each feature
3. Commit changes with clear messages
4. Submit a pull request for review

## License

This project is open-source and licensed under the **MIT License**.

### Why MIT License?
The MIT License was chosen because it provides freedom to use, modify, and distribute the project with minimal restrictions, making it accessible for developers to contribute and innovate.

## Issue Tracker

We use GitHub Issues to track bugs and enhancements. You can report a bug or suggest a feature [here](https://github.com/ntran5518/Absolute_Value_Project/issues).

### Current Open Issue:
- **Enhancement Request:** Implement dark mode for improved accessibility. (Issue #1)

## Project Wiki

We have a dedicated **[Project Wiki](https://github.com/ntran5518/Absolute_Value_Project/wiki)** that includes detailed documentation about our version control strategy.

### Version Control Strategy

We use **Git with GitHub** as our version control system.

#### Why GitHub?
1. **Collaboration & Branching:** GitHub allows multiple team members to work simultaneously with effective branching strategies.
2. **Pull Requests & Code Review:** Built-in pull request and review features improve code quality.
3. **Integration & Deployment:** GitHub Actions enables automated testing and continuous integration.
