Test Case ID: TC_LOGIN_001
Test Scenario: Verify login with valid credentials
Precondition: User account must already exist
Test Steps:
    1. Open the login page
    2. Enter a valid username/email
    3. Enter a valid password
    4. Click the login button
Test Data: Valid username/email and valid password
Expected Result: User should be logged in successfully and redirected to the appropriate page
Actual Result: The user was successfully logged in and redirected to the My Account page
Status: Pass


Test Case ID: TC_LOGIN_002
Test Scenario: Verify login with invalid password
Precondition: User account must already exist
Test Steps:
    1. Open the login page
    2. Enter a valid username/email
    3. Enter a invalid password
    4. Click the login button
Test Data: Valid username/email and invalid password
Expected Result: User should not be logged in and an appropriate error message should be displayed
Actual Result: The login attempt was rejected and the message "Invalid email or password" was displayed
Status: Pass


Test Vase ID: TC_LOGIN_003
Test Scenario: Verify login with invalid email/username
Precondition: Login page must be available
Test Steps:
    1. Open the login page
    2. Enter a invalid username/email
    3. Enter any password
    4. Click the login button
Test Data: Invalid username/email
Expected Result: User should not be logged in and appropriate error message should be displayed
Actual Result: The login attempt was rejected and the message "Invalid email or password" was displayed
Status: Pass


Test Vase ID: TC_LOGIN_004
Test Scenario: Verify login with empty required fields
Precondition: Login page must be available
Test Steps:
    1. Open the login page
    2. Leave username/email empty
    3. Leave password empty
    4. Click the login button
Test Data: Empty username/email and password
Expected Result: User should not be logged in and required field validation messages should be displayed
Actual Result: The login attempt was rejected. The message "Email is required" was displayed and the user remained on the login page
Status: Pass


Test Vase ID: TC_LOGIN_005
Test Scenario: Verify password visibility bahavior
Precondition: Login page must be available
Test Steps:
    1. Open the login page
    2. Enter a valid username/email
    3. Leave password empty
    4. Click the login button
Test Data: Valid username/email and empty password
Expected Result: User should not be logged in and a password validation message should be displayed
Actual Result: The login attempt was rejected. The message "Password is required" was displayed and the user remained on the login page
Status: Pass
