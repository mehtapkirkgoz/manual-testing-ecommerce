Test Case ID: TC_REG_001
Test Scenario: Verify registration with valid user information
Precondition: Registration page must be available and email address must not be registered before
Test Steps:
    1. Open the registration page
    2. Enter valid user information
    3. Enter a valid email address
    4. Enter a valid password
    5. Confirm the password
    6. Click the Register button
Test Data: Valid name, valid email address, valid password
Expected Result: User account should be created successfully
Actual Result: The user account was created successfully with valid information
Status: Pass


Test Case ID: TC_REG_002
Test Scenario: Verify registration with an already registered email address
Precondition: An account with the same email address must already exist
Test Steps:
    1. Open the registration page
    2. Enter valid user information
    3. Enter an already registered email address
    4. Enter a valid password
    5. Confirm the password
    6. Click the Register button
Test Data: Existing email address and valid password
Expected Result: User account should not be created and an appropriate error message should be displayed
Actual Result: The registration attempt was rejected and the message "A customer with this email address already exists." was displayed
Status: Pass


Test Case ID: TC_REG_003
Test Scenario: Verify registration with empty required fields
Precondition: Registration page must be available
Test Steps:
    1. Open the registration page
    2. Leave the required fields empty
    3. Click the Register button
Test Data: Empty required fields 
Expected Result: User account should not be created and validation messages should be displayed for the required fields
Actual Result: The registration attempt was rejected. Validation messages were displayed under each required field, indicating that the field is required
Status: Pass


Test Case ID: TC_REG_004
Test Scenario: Verify registration with invalid email format
Precondition: Registration page must be available
Test Steps:
    1. Open the registration page
    2. Enter valid user information
    3. Enter an email address in an invalid format
    4. Enter a valid password
    5. Confirm the password
    6. Click the Register button
Test Data: Invalid email format and valid password
Expected Result: User account should not be created and an appropriate validation message should be displayed for the email field
Actual Result: The registration attempt was rejected and the message "Invalid email format" was displayed
Status: Pass


Test Case ID: TC_REG_005
Test Scenario: Verify password and confirm password mismatch behavior
Precondition: Registration page must be available
Test Steps:
    1. Open the registration page
    2. Enter valid user information
    3. Enter a valid email 
    4. Enter a valid password
    5. Enter a different password in the Confirm Password field
    6. Click the Register button
Test Data: Valid email address, valid password, and different confirm password
Expected Result: User account should not be created and an appropriate validation message should indicate that the passwords do not match
Actual Result: The application does not contain a Confirm Password field
Status: Not Applicable
Note: This test case is not applicable because the registration form only contains one password field


Test Case ID: TC_REG_006
Test Scenario: Verify password validation rules
Precondition: Registration page must be available
Test Steps:
    1. Open the registration page
    2. Enter valid user information
    3. Enter a valid email
    4. Enter a password without a special symbol
    5. Click the Register button
Test Data: Mhtp1234
Expected Result: User account should not be created and a validation message should indicate that the password must contain at least one special symbol
Actual Result: The registration attempt was rejected, but the message "Password must not contain invalid characters" was displayed
Status: Fail
Related Bug: BUG_001