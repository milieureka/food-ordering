# Food Ordering System 🍔🍕🥗

![Order Function](https://github.com/milieureka/food-ordering/blob/main/access/003-image.jpg)
![Add to Cart Function](https://github.com/milieureka/food-ordering/blob/main/access/004-image.jpg)
![Checkout Process](https://github.com/milieureka/food-ordering/blob/main/access/005-image.jpg)

## Overview
This project is a web-based food ordering system that incorporates various functionalities such as filtering items, adding items to a cart, checking out, and user authentication (signup/login). 

---

## Tutorial 📚

### Filter Function
1. **Event Listener for Document Loading**:
   - Ensures all elements are loaded before execution.
2. **Selecting Elements**:
   - Uses `document.querySelector` to access HTML elements like menu body, filters, and buttons.
3. **Filter Button Click Event Listener**:
   - Executes filtering and sorting logic upon button click.
4. **Retrieving Selected Filter Values**:
   - Reads user preferences from dropdown menus.
5. **Filtering and Sorting Items**:
   - Converts menu items into an array, filters based on criteria, and sorts by price.
6. **Updating the DOM**:
   - Dynamically refreshes the menu display without page reload.

---

### Add to Cart Function
1. **HTML Integration**:
   - "Add to Cart" button on each menu item.
2. **JavaScript Logic**:
   - **Event Listener on DOMContentLoaded**:
     - Activates after DOM content loads.
   - **Adding to Cart**:
     - Captures item data, creates objects, and updates cart UI and storage.
   - **Quantity Control**:
     - Provides `+` and `-` buttons for adjusting quantities.
   - **Total Price Calculation**:
     - Accumulates prices and dynamically updates the total.
   - **Checkout Button**:
     - Clears the cart after a successful checkout.

---

### Checkout Function
1. **Initializing the Cart Page**:
   - Loads cart items from local storage.
   - Targets and updates the cart display elements.
2. **Displaying Cart Items**:
   - Iterates through cart items to create a table of items.
3. **Calculating Prices**:
   - Subtotal is calculated using `reduce`.
   - Total price includes shipping and is updated in the UI.
4. **Checkout Form Submission**:
   - Handles form submissions and prepares for backend integration.

---

### Search Function
- Integrates a search route to fetch and display items from the database based on user input.

---

### Signup & Login Function
#### Signup
- **Endpoint**: `POST /signup`
- **Purpose**: Registers new users.
- **Process**:
  - Extracts and validates `userID` and password.
  - Inserts data into `foodUsers` database.
  - Sends a success or error message based on result.

#### Login
- **Endpoint**: `POST /login`
- **Purpose**: Authenticates users.
- **Process**:
  - Retrieves `userID` and password.
  - Validates against the database.
  - Redirects to the homepage on success or returns an error on failure.

---

## How to Run 🚀
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo-name.git
