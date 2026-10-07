Test Case ID: TC_CART_001
Test Scenario: Verify a product can be added to the shopping cart
Precondition: The application must be available and at least one product must be available
Test Steps:
    1. Open the application
    2. Select a product
    3. Click the Add to Cart button
    4. Open the shopping cart
Test Data: Existing product
Expected Result: The selected product should be added to the shopping cart successfully
Actual Result: The selected product was added to the shopping cart successfully
Status: Pass


Test Case ID: TC_CART_002
Test Scenario: Verify multiple products can be added to the cart
Precondition: The application must be available and at least two products must be available
Test Steps:
    1. Open the application
    2. Select a product
    3. Click the Add to Cart button
    4. Select another product
    5. Click the Add to Cart button
    6. Open the shopping cart
Test Data: Two existing products
Expected Result: Both selected products should be added to the shopping cart successfully
Actual Result: Both selected product were added to the shopping cart successfully
Status: Pass 


Test Case ID: TC_CART_003
Test Scenario: Verify product quantity can be decreased
Precondition: The application must be available, the product must be in stock, and the shopping cart must contain at least two units of the same product
Test Steps:
    1. Open the application
    2. Open the Shopping cart
    3. Locate the product with quantity 2 or more
    4. Click the decrease quantity button
    5. Observe the product quantity and cart total
Test Data: Product quantity: 2
Expected Result: The product quantity should decrease by one and the cart total should be updated correctly
Actual Result: The product quantity was decreased successfully and the cart total was updated correctly
Status: Pass


Test Case ID: TC_CART_004
Test Scenario: Verify a product can be removed from the cart
Precondition: The application must be available and at least one product must be in the shopping cart
Test Steps:
    1. Open the application
    2. Open the Shopping cart
    3. Locate the product you want to remove
    4. Click the Remove button
Test Data: Existing product in the shopping cart
Expected Result: The product should be removed from the shopping cart and the cart total should be updated correctly
Actual Result: The product was removed from the shopping cart and the cart total was updated correctly
Status: Pass


Test Case ID: TC_CART_005
Test Scenario: Verify the cart total is calculated correctly
Precondition: The application must be available and at least one product must be in the shopping cart.
Test Steps:
    1. Open the application.
    2. Open the shopping cart.
    3. Check the unit price of the product.
    4. Check the product quantity.
    5. Calculate the expected total price manually.
    6. Compare the calculated amount with the cart total.
Test Data: Product unit price and quantity.
Expected Result: The cart total should be equal to the product unit price multiplied by the selected quantity.
Actual Result: The cart total matched the manually calculated expected total
Status: Pass


Test Case ID: TC_CART_006
Test Scenario: Verify cart contents are retained while navigating between pages
Precondition: The application must be available and at least one product must be in the shopping cart
Test Steps:
    1. Open the application
    2. Open the Shopping cart
    3. Verify that there is at least one item in the shopping cart.
    4. Navigate to different pages of the application
    5. Open the Shopping cart
    6. Confirm that the contents of the shopping cart are still the same
Test Data: At least one product in the shopping cart
Expected Result: The shopping cart contents are preserved when navigating between pages
Actual Result: The shopping cart contents were preserved while navigating between pages
Status: Pass


Test Case ID: TC_CART_007
Test Scenario: Verify shopping cart contents are synchronized across browser tabs
Precondition: The user must be logged in and at least one product must be in the shopping cart
Test Steps:
    1. Open the application
    2. Add a product to the shopping cart
    3. Verify that the product is visible in the cart.
    4. Open the application in a new browser tab
    5. Open the shopping cart in the new tab
    6. Compare the cart contents between both tabs
Test Data: At least one product in the shopping cart
Expected Result: The shopping cart contents should be consistent across browser tabs for the same logged-in user
Actual Result: The product was visible in the original tab but was not visible in the new tab
Status: Fail
Related Bug: BUG_002