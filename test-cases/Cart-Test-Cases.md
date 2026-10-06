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
Status: Not Run 


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
Status: Not Run 


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
Status: Not Run


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
Status: Not Run


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
Status: Not Run


Test Case ID: TC_CART_006
Test Scenario: Verify cart contents are retained while navigating between pages
Precondition: The application must be available and at least one product must be in the shopping cart
Test Steps:
    1. Open the application
    2. Open the Shopping cart
    3. Verify that there is at least one item in the shopping cart.
    4. randomly browse through the pages
    5. Open the Shopping cart
    6. Confirm that the contents of the shopping cart are still the same
Test Data: At least one product in the shopping cart
Expected Result: The shopping cart contents are preserved when navigating between pages
Status: Not Run