## Bug Report: Login allows empty password field

**ID:** BUG-001  
**Project:** Sauce Demo  
**Reported by:** Liziel Almanon
**Date:** 2025-12-08  
**Environment:**  
- Browser: Chrome 112.0  
- OS: Windows 10  
- Device: Desktop  
- App Version: 1.0.0  

---

### Summary  
The login form allows submission with an empty password field, letting users proceed without entering a password.

---

### Description  
When a user attempts to login with a valid username but leaves the password field empty and clicks the Login button, the system does not block the login attempt or show an appropriate error message. Instead, it allows submission which results in unexpected behavior or error downstream.

---

### Steps to Reproduce  
1. Navigate to the login page.  
2. Enter a valid username in the username field.  
3. Leave the password field empty.  
4. Click the Login button.  

---

### Expected Result  
An error message should be displayed indicating that the password field is required and login should be blocked until a password is entered.

---

### Actual Result  
No error message is shown, and the form submission proceeds with an empty password.

---

### Screenshots / Videos  
![Login empty password](https://example.com/screenshots/bug-login-empty-password.png)  

---

### Severity  
Medium  

---

### Priority  
High  

---

## Bug Report: Login with locked-out user does not show proper error message

**ID:** BUG-002  
**Project:** Sauce Demo  
**Reported by:** Liziel Almanon
**Date:** 2025-12-08  
**Environment:**  
- Browser: Firefox 114.0  
- OS: Windows 10  
- Device: Desktop  
- App Version: 1.0.0  

---

### Summary  
Attempting to login with a locked-out user does not show the expected lockout error message.

---

### Description  
When a user with locked-out credentials tries to login, the system fails to display the specific error message indicating that the user has been locked out. Instead, it shows a generic error message that confuses users.

---

### Steps to Reproduce  
1. Go to the login page.  
2. Enter locked-out username.  
3. Enter valid password.  
4. Click Login.  

---

### Expected Result  
An error message clearly stating that the user has been locked out is displayed.

---

### Actual Result  
A generic login failure message is displayed instead.

---

### Screenshots / Videos  
![Locked-out error message](https://example.com/screenshots/bug-lockedout-message.png)  

---

### Severity  
High  

---

### Priority  
High  

---

### Additional Notes  
Proper error messaging improves user experience and reduces support tickets.


---

## Bug Report: Add-to-cart allows duplicate items

**ID:** BUG-003  
**Project:** Sauce Demo  
**Reported by:** Liziel Almanon  
**Date:** 2025-12-08  
**Environment:**  
- Browser: Edge 112.0  
- OS: Windows 11  
- Device: Desktop  
- App Version: 1.0.0  

---

### Summary  
Clicking “Add to Cart” multiple times adds the same item multiple times instead of once.

---

### Description  
Users can add the same product to the cart multiple times by clicking the "Add to Cart" button repeatedly. The cart badge increments each time, but the product list in the cart duplicates the item instead of increasing quantity or blocking duplicates.

---

### Steps to Reproduce  
1. Login and navigate to the product listing page.  
2. Select a product.  
3. Click the Add to Cart button multiple times.  
4. Open the cart.  

---

### Expected Result  
The product should only be added once or quantity should increase instead of duplicating items.

---

### Actual Result  
Multiple instances of the same product appear in the cart list.

---

### Screenshots / Videos  
![Add to cart duplicate](https://example.com/screenshots/bug-addtocart-duplicate.png)  

---

### Severity  
Medium  

---

### Priority  
Medium  

---

### Additional Notes  
Fixing this will improve cart accuracy and user experience.

---

## Bug Report: Checkout allows empty first name input

**ID:** BUG-004  
**Project:** Sauce Demo  
**Reported by:** Liziel Almanon
**Date:** 2025-12-08  
**Environment:**  
- Browser: Chrome 112.0  
- OS: macOS Monterey  
- Device: Laptop  
- App Version: 1.0.0  

---

### Summary  
Users can proceed with checkout leaving the First Name field empty in the delivery information form.

---

### Description  
The checkout form does not validate the First Name field properly. Users are allowed to submit the form without entering a first name, which leads to incomplete order details and potential processing errors.

---

### Steps to Reproduce  
1. Login and add an item to cart.  
2. Go to checkout page.  
3. Leave the First Name field empty.  
4. Fill out the rest of the delivery and payment information.  
5. Attempt to complete checkout.  

---

### Expected Result  
An error message should prompt the user to fill in the First Name field, blocking submission until corrected.

---

### Actual Result  
Checkout proceeds without any error despite missing First Name.

---

### Screenshots / Videos  
![Checkout empty first name](https://example.com/screenshots/bug-checkout-empty-firstname.png)  

---

### Severity  
High  

---

### Priority  
High  

---

### Additional Notes  
This bug could cause issues with shipping and customer communication. Input validation needed.

---

### Additional Notes  
This issue could lead to potential authentication bypass or cause errors on backend services. Recommend adding client-side and server-side validation for required fields.
