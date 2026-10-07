Example 1: Email Field Validation

Requirement: The email field should accept valid ameil addresses and reject invalid email formats

Equivalance Partitions:

    Partition | Description | Example Test Data | Expected Result
   1: Valid | Properly formatted email address | test@example.com | Email should be accepted
   2: Invalid | Missing Domain | test@ | Email should be rejected
   3: Invalid | Missing @ symbol | testexample.com | Email should be rejected
   4: Invalid | Missing user name | @example.com | Email should be rejected 



Example 2: Password Validation

Requirement: The password must meet all defined password rules

Equivalence Partitions:

    Partition | Description | Example Test Data | Expected Result
   1: Valid | Meets all password rules | Test.1234 | Accepted
   2: Invalid | Less than 8 characters | Test.1 | Rejected
   3: Invalid | Missing uppercase letter | test.1234 | Rejected
   4: Invalid | Missing lowercase letter | TEST.1234 | Rejected
   5: Invalid | Missing number | Test.example | Rejected
   6: Invalid | Missing special symbol | Test1234 | Rejected 