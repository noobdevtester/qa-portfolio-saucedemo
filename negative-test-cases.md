Negative Test Cases – Sauce Demo

**TC-005: Verify login with empty credentials**  
**Precondition:** User is on login page  
**Steps:**
  1. Leave Username field empty  
  2. Leave Password field empty  
  3. Click Login  

**Expected Result:** Error message is displayed indicating that username is required & login is blocked  
**Status:** Pass  

**TC-006: Verify login with invalid credentials**  
**Precondition:** User is on login page  
**Steps:**
  1. Enter invalid username  
  2. Enter invalid password  
  3. Click Login  

**Expected Result:** System displays an error message stating that the username & password do not match any user  
**Status:** Pass  

**TC-007: Verify login with locked-out user**  
**Precondition:** User is on login page  
**Steps:**
  1. Enter locked-out username  
  2. Enter valid password  
  3. Click Login  

**Expected Result:** Error message is displayed indicating that the user has been locked out  
**Status:** Pass  

**TC-008: Verify add-to-cart without user authentication**  
**Precondition:** User is not authenticated  
**Steps:**
  1. Navigate directly to the product listing page URL  
  2. Click Add to Cart button for any product  

**Expected Result:** User is redirected to the login page & the item is not added to the cart  
**Status:** Pass  

**TC-009: Verify adding the same item to cart multiple times**  
**Precondition:** User is authenticated & viewing the item list page  
**Steps:**
  1. Select a product from the item list page  
  2. Click the Add to Cart button multiple times  

**Expected Result:** Item is added only once & the cart icon badge displays the correct number of items  
**Status:** Pass  

**TC-010: Verify checkout with empty first name**  
