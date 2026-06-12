QA CAPSTONE PROJECT – REGISTRATION & LOGIN SYSTEM TESTING


1. PROJECT TEST PLAN


Objective:

Verify that the registration and login system works correctly and meets the required functionality.


Scope:


- Registration

- Login

- Password validation

- Email validation

- Forgot password functionality


Testing Strategy:


- Functional Testing

- Boundary Value Analysis (BVA)

- Equivalence Partitioning (EP)

- Regression Testing


2. REQUIREMENT TRACEABILITY MATRIX (RTM)


Requirement ID: R001

Requirement: User can register

Test Cases: TC001, TC002


Requirement ID: R002

Requirement: User logs in

Test Cases: TC003, TC004


Requirement ID: R003

Requirement: Email validation

Test Cases: TC005


Requirement ID: R004

Requirement: Password rules

Test Cases: TC006


Requirement ID: R005

Requirement: Forgot password

Test Cases: TC007


3. TEST CASES


TC001

Scenario: Register with valid details

Expected Result: Account created successfully

Status: Pass


TC002

Scenario: Register with empty fields

Expected Result: Validation error displayed

Status: Pass


TC003

Scenario: Login with valid credentials

Expected Result: User logged in successfully

Status: Pass


TC004

Scenario: Login with invalid password

Expected Result: Error message displayed

Status: Pass


TC005

Scenario: Invalid email format

Expected Result: Email rejected

Status: Pass


TC006

Scenario: Password under 8 characters

Expected Result: Validation message displayed

Status: Fail


TC007

Scenario: Forgot password link

Expected Result: Reset email sent

Status: Pass


TC008

Scenario: Username with special characters

Expected Result: Input rejected

Status: Pass


TC009

Scenario: Blank login fields

Expected Result: Validation message displayed

Status: Pass


TC010

Scenario: Session timeout

Expected Result: Redirect to login page

Status: Fail


4. DEFECTS / BUG REPORTS


Bug ID: BUG001

Description: Password accepts less than 8 characters

Severity: High

Priority: High


Bug Details:

Steps to Reproduce:


1. Open registration page

2. Enter password: "12345"

3. Click Submit


Expected Result:

System should reject weak passwords.


Actual Result:

Account was created successfully.


Bug ID: BUG002

Description: Session timeout not working

Severity: Medium

Priority: High


Bug Details:

Steps to Reproduce:


1. Login

2. Stay inactive for 20 minutes


Expected Result:

User should be redirected to login page.


Actual Result:

Session remains active.


5. CONCLUSION


Total Test Cases Executed: 10


Passed: 8


Failed: 2


Summary:

Two defects were identified and successfully reported during testing. The testing process helped validate core registration and login functionalities while identifying critical issues requiring fixes.
