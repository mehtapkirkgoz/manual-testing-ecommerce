Bug ID: BUG_001
Title: Incorrect validation message is displayed when the password does not contain a special symbol

Environment:
Windows 11
Google Chrome
Practice Software Testing

Precondition: Registration page must be available.

Steps to Reproduce:
    1. Open the registration page.
    2. Enter valid user information.
    3. Enter a valid email address.
    4. Enter "Mhtp1234" in the password field.
    5. Click the Register button.

Actual Result: The registration attempt is rejected and the message
"Password must not contain invalid characters"
is displayed.

Expected Result: The registration attempt should be rejected and a validation message should clearly indicate that the password must contain at least one special symbol.

Evidence:
![BUG_001 Password Validation](./evidence/BUG_001-password-validation.png)

Severity:
Low

Priority:
Medium

Status:
Open


Bug ID: BUG_002

Title: Shopping cart contents are not synchronized across browser tabs

Environment:
Windows 11
Google Chrome
Practice Software Testing

Precondition: 
-User must be logged in
-At least one product must be added to the shopping cart

Steps to Reproduce:
    1. Login to the application
    2. Add a product to the shopping cart
    3. Open the shopping cart in the current tab and verify that the product in visible
    4. Open the application in a new browser tab
    5. Navigate to the shopping cart in the new tab
    6. Return to the original tab and check the shopping cart again

Actual Result: The product is visible in the iriginal tab, but the shopping cart isn't visible in the new tab. When returning to the original tab, the product is still visible

Expected Result: The shopping cart contents should remain consistent across browser tabs for the same logged-in user session

Additional Observation:
Authentication state is synchronized across browser tabs after refresh, but shopping cart contents are not.

Severity: Medium

Priority: Medium

Status: Open

Related Test Case: TC_CART_006


Bug ID: BUG_003

Title: Registered user account is no longer recognized after session expiration

Environment:
Windows 11
Google Chrome
Practice Software Testing

Precondition: A valid customer account must already exist

Steps to Reproduce:
    1. Register a new customer account
    2. Log in successfully with the registered email and password
    3. Wait until the session expires and the user is logged out automatically
    4. Attempt to log in again using the same email and password
    5. Observe the login result
    6. Navigate to the registration page 
    7. Enter different personal information but use the same email address and password
    8. Submit the registration form

Actual Result: 
-The existing credentials are rejected with the message 'Invalid email or password'
-The same email address can the be used to register a new account successfully

Expected Result: The existing accound should remain available after session expiration. The ıuser should be able to log in again using the same valid credentials, and the same email address should not be accepted for a new registration.

Severity: High

Priority: High

Status: Open

Reproducibility: Reproduced more than once