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
Status: Not Run


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
Status: Not Run


Test Case ID: TC_REG_003
Test Scenario: Verify registration with empty required fields
Precondition: Registration page must be available
Test Steps:
    1. Open the registration page
    2. Leave the required fields empty
    3. Click the Register button
Test Data: Empty required fields 
Expected Result: User account should not be created and validation messages should be displayed for the required fields
Status: Not Run


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
Status: Not Run


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
Status: Not Run