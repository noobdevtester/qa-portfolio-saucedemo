## Positive Test Cases – Sauce Demo

TC-001: Verify Sign-Up with valid credentials
**Precondition:** User is on sign-up page  
**Steps:**
1. Enter valid first name
2. Enter valid last name
3. Enter valid e-mail address
4. Enter password
5. Click Create Button

**Expected Result:** User is successfully redirected to product listing page and email is received for confirmation of sign-up
**Status:** Pass

### TC-002: Verify Login with valid credentials
**Precondition:** User is on login page  
**Steps:**
1. Enter valid email
2. Enter valid password
3. Click Login

**Expected Result:** User is successfully redirected to account details and order history
**Status:** Pass

### TC-003: Verify add-to-cart functionality
**Precondition:** User is authenticated and viewing the item list page
**Steps:**
1. Select an item from the item list page.
2. Click the Add to Cart button for the selected product.

**Expected Result:** The selected item is added to the cart, and the cart icon badge displays the correct number of items.
**Status:** Pass

### TC-004: Verify check-out functionality for a single item
**Precondition:** User is authenticated and has one item added to the cart.
**Steps:**
1. Navigate to My Cart page.
2. Verify that the item name, price, quantity, and total amount are correct.
3. Click the Checkout button.
4. Enter valid delivery information (First Name, Last Name, Address).
5. Enter valid payment information (Card number, Expiration Date Security Code, Name on card).
6. Enter shipping information
7. Click Pay Now Button

**Expected Result:** User is redirected to the checkout overview page displaying correct item and total details.
**Status:** Pass
