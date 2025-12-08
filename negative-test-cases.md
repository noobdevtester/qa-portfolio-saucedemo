Negative Test Cases – Sauce Demo
TC-005: Verify login with empty credentials

Precondition: User is on login page
Steps:

Leave Username field empty

Leave Password field empty

Click Login

Expected Result: Error message is displayed indicating that username is required & login is blocked
Status: Pass

TC-006: Verify login with invalid credentials

Precondition: User is on login page
Steps:

Enter invalid username

Enter invalid password

Click Login

Expected Result: System displays an error message stating that the username & password do not match any user
Status: Pass

TC-007: Verify login with locked-out user

Precondition: User is on login page
Steps:

Enter locked-out username

Enter valid password

Click Login

Expected Result: Error message is displayed indicating that the user has been locked out
Status: Pass

TC-008: Verify add-to-cart without user authentication

Precondition: User is not authenticated
Steps:

Navigate directly to the product listing page URL

Click Add to Cart button for any product

Expected Result: User is redirected to the login page & the item is not added to the cart
Status: Pass

TC-009: Verify adding the same item to cart multiple times

Precondition: User is authenticated & viewing the item list page
Steps:

Select a product from the item list page

Click the Add to Cart button multiple times

Expected Result: Item is added only once & the cart icon badge displays the correct number of items
Status: Pass

TC-010: Verify checkout with empty first name

Precondition: User is authenticated & has one item added to the cart
Steps:

Navigate to My Cart page

Click the Checkout button

Leave First Name field empty

Enter valid Last Name & Postal Code

Click Continue

Expected Result: Error message is displayed indicating that First Name is required & checkout does not proceed
Status: Pass

TC-011: Verify checkout with empty postal code

Precondition: User is authenticated & has one item added to the cart
Steps:

Navigate to My Cart page

Click the Checkout button

Enter valid First Name & Last Name

Leave Postal Code field empty

Click Continue

Expected Result: Error message is displayed indicating that Postal Code is required & checkout is blocked
Status: Pass

TC-012: Verify checkout with empty cart

Precondition: User is authenticated & cart is empty
Steps:

Navigate to My Cart page

Click the Checkout button

Expected Result: System prevents checkout & displays a message indicating that the cart is empty
Status: Pass

TC-013: Verify session handling after logout

Precondition: User is logged in
Steps:

Click Logout

Press the browser Back button

Expected Result: User remains logged out & restricted pages are not accessible
Status: Pass
