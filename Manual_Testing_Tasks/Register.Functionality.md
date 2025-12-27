# **MANUAL TESTING TASK ASSIGNMENT**

##### **Project:** `Automation Exercise E-commerce Platform`
##### **Module:** `Signup/Registration Page Testing`
##### **Document ID:** `QA-TASK-AUTOEX-SIGNUP-001`
##### **Priority:** `High`
##### **Assigned To:** `Pranav Ranamale`
##### **Estimated Effort:** `3-4 hours`

---

## **1. TASK OVERVIEW**
You have been assigned to perform comprehensive manual testing on the New User Signup page of the Automation Exercise e-commerce platform. Based on the provided UI screenshot, you are required to design, execute, and document test scenarios covering functional, UI/UX, validation, security, and usability aspects of the user registration functionality.

## **2. TEST OBJECTIVE**
Validate that the New User Signup page functions correctly according to specifications, provides secure user registration, offers intuitive user experience, and handles all possible user interactions appropriately for new user registration.

## **3. SCOPE OF TESTING**
**In-Scope:** Signup form functionality (via "Signup / Login" button), UI/UX elements verification, Input field validations (Name & Email), Registration logic, Navigation elements, Error handling mechanisms, Security aspects, Responsive behavior, Email verification flow.

**Out-of-Scope:** Backend API testing, Performance/Load testing, Database validation, Third-party integrations, Mobile application testing, Login functionality, Product listing/cart functionality.

## **4. TEST ENVIRONMENT DETAILS**
- **Base URL:** https://automationexercise.com
- **Signup Page URL:** https://automationexercise.com/login
- **Browser Compatibility:** Chrome v115+, Firefox v110+, Edge v115+
- **Screen Resolutions:** 1920x1080, 1366x768, 1536x864, 375x667

## **5. MANDATORY TEST SCENARIOS**

### **SCENARIO 1: NAVIGATION TO SIGNUP PAGE**
**Objective:** Verify proper navigation from homepage to signup page.

1. Navigate from homepage to signup page via "Signup / Login" button
2. Verify signup page URL is correct
3. Verify page title contains "Automation Exercise"
4. Verify user is on right section of login/signup page
5. Verify browser back button returns to homepage

### **SCENARIO 2: UI ELEMENTS VERIFICATION**
**Objective:** Verify all UI elements are present and properly aligned.

1. Verify "New User Signup!" heading is displayed
2. Verify "Name" field with label is present
3. Verify "Email Address" field with label is present
4. Verify "Signup" button is present and enabled
5. Verify "Login to your account" section is visible on left
6. Verify header navigation elements (Home, Products, Cart, Contact us)
7. Check all text spelling and grammar
8. Verify font consistency across page
9. Verify field placeholder text (if any)
10. Verify required field indicators (asterisks, if present)

### **SCENARIO 3: FUNCTIONAL VALIDATION - POSITIVE FLOW**
**Objective:** Validate successful new user registration.

1. Register with valid unique name and email address
2. Verify successful form submission
3. Verify redirection to account information page after signup
4. Verify confirmation message appears
5. Verify email verification requirement (if applicable)
6. Verify auto-login after successful registration
7. Verify new user appears in system
8. Verify welcome email received (if applicable)

### **SCENARIO 4: FUNCTIONAL VALIDATION - NEGATIVE FLOW**
**Objective:** Validate error handling for invalid registration attempts.

1. Register with already registered email address
2. Register with invalid email format
3. Register with empty name field
4. Register with empty email field
5. Register with both fields empty
6. Register with name containing only spaces
7. Register with email containing only spaces
8. Verify appropriate error messages display
9. Verify error message disappears on field focus
10. Verify duplicate registration prevention

### **SCENARIO 5: INPUT FIELD VALIDATIONS - NAME FIELD**
**Objective:** Validate name field constraints and behaviors.

1. Verify minimum name length acceptance
2. Verify maximum name length handling
3. Verify special character handling in name
4. Verify numeric characters in name
5. Verify space character handling in name
6. Verify copy-paste functionality
7. Verify trim leading/trailing spaces
8. Verify case preservation
9. Verify international character support

### **SCENARIO 6: INPUT FIELD VALIDATIONS - EMAIL FIELD**
**Objective:** Validate email field constraints and behaviors.

1. Verify valid email format acceptance
2. Verify invalid email format rejection
3. Verify maximum character limit
4. Verify email case sensitivity (should be case-insensitive)
5. Verify copy-paste functionality
6. Verify space character handling
7. Verify autocomplete behavior
8. Verify disposable email detection (if implemented)

### **SCENARIO 7: DUPLICATE REGISTRATION HANDLING**
**Objective:** Validate prevention of duplicate user registrations.

1. Attempt registration with existing email address
2. Attempt registration with existing email in different case
3. Attempt registration with email containing extra spaces
4. Verify clear error message for duplicate registration
5. Verify suggestion to use "Forgot Password" instead
6. Verify redirect to login page option
7. Verify system doesn't create duplicate accounts

### **SCENARIO 8: SECURITY TESTING**
**Objective:** Validate security aspects of the registration mechanism.

1. Verify HTTPS protocol usage on signup page
2. Verify form submission encryption
3. Test SQL injection attempts in name/email fields
4. Test XSS payloads in name/email fields
5. Verify CAPTCHA implementation (if present)
6. Verify rate limiting for registration attempts
7. Verify no sensitive data exposure in page source
8. Verify CSRF token implementation

### **SCENARIO 9: DATA PERSISTENCE & VALIDATION**
**Objective:** Validate data persistence during registration flow.

1. Verify entered data persists on form validation error
2. Verify data clears after successful submission
3. Verify browser refresh retains entered data
4. Verify back navigation retains form data
5. Verify form data lost after session timeout
6. Verify field focus retention on error
7. Verify input trimming before validation

### **SCENARIO 10: NAVIGATION & LINKS**
**Objective:** Validate all navigation elements and links.

1. Verify "Signup" button functionality and state changes
2. Verify "Login to your account" section link functionality
3. Verify header "Home" link navigation
4. Verify header "Products" link navigation
5. Verify header "Cart" link navigation
6. Verify header "Contact us" link navigation
7. Verify "Test Cases" link functionality
8. Verify "API Testing" link functionality
9. Verify browser refresh during registration process

### **SCENARIO 11: USABILITY & ACCESSIBILITY**
**Objective:** Validate user-friendly experience and accessibility compliance.

1. Verify tab navigation order: Name → Email → Signup
2. Verify Enter key submits registration form
3. Verify field auto-focus on page load
4. Verify keyboard-only navigation
5. Verify screen reader compatibility
6. Verify color contrast ratios (WCAG compliance)
7. Verify responsive design on different screen sizes
8. Verify error message clarity and helpfulness
9. Verify form labels are properly associated

### **SCENARIO 12: EDGE CASES & EXPLORATORY**
**Objective:** Identify unexpected behaviors and edge conditions.

1. Register with extremely long name (100+ characters)
2. Register with extremely long email address
3. Submit form multiple times quickly (double-click prevention)
4. Register during network interruption
5. Change URL parameters during registration process
6. Test with browser zoom (80%, 100%, 125%, 150%)
7. Test with browser developer tools open
8. Test with ad-blockers enabled
9. Test with cookies disabled
10. Test with JavaScript disabled

### **SCENARIO 13: EMAIL VERIFICATION FLOW**
**Objective:** Validate email verification process (if implemented).

1. Verify email is sent after registration
2. Verify email content accuracy
3. Verify verification link functionality
4. Verify expired link handling
5. Verify already verified link handling
6. Verify resend verification email functionality
7. Verify account status before/after verification

### **SCENARIO 14: BROWSER COMPATIBILITY**
**Objective:** Verify consistent behavior across browsers.

1. Test signup functionality on Chrome latest
2. Test signup functionality on Firefox latest
3. Test signup functionality on Edge latest
4. Verify responsive design across browsers
5. Verify error message display consistency
6. Verify form submission behavior consistency
7. Verify validation behavior consistency

### **SCENARIO 15: POST-REGISTRATION FLOW**
**Objective:** Validate user experience after successful registration.

1. Verify redirection to appropriate page
2. Verify welcome message/notification
3. Verify user is automatically logged in
4. Verify account information page accessibility
5. Verify dashboard/account page elements
6. Verify logout functionality
7. Verify login with newly created credentials

## **6. DELIVERABLES REQUIREMENTS**
**Mandatory Deliverables:**
1. Test Execution Report (Excel/Google Sheets format)
2. Defect/Bug Report (For each failure found)
3. Test Summary Report (Overall execution summary)

**Format Specifications:**
- Use test case naming convention: `AUTOEX-SIGNUP-TC-001`
- Save screenshots as: `AUTOEX-SIGNUP-SCR-YYYYMMDD-HHMMSS.png`
- Submit all documents in: `AUTOEX-SIGNUP-REPORT-YYYYMMDD.zip`

## **7. ACCEPTANCE CRITERIA**
The task will be considered **COMPLETE** when:
- All mandatory scenarios are executed
- Minimum 95% test case pass rate achieved
- All critical/severe defects logged and documented
- All deliverables submitted in specified format
- Test evidence (screenshots) provided for all test cases
- Exploratory testing conducted for at least 30 minutes
- Cross-browser testing completed on 2+ browsers

## **8. ADDITIONAL NOTES**
**Assumptions:**
- Test environment is stable and accessible
- Temporary email services are available for testing
- No major changes to UI during testing period

**Risks:**
- Environment downtime may impact testing
- Email delivery delays may block verification tests
- Browser compatibility issues may occur

**Dependencies:**
- Access to test environment
- Availability of test email accounts
- Functional requirements document

**Escalation Point:** Team Lead/QA Manager for any blocking issues

## **9. SUBMISSION DETAILS**
**Due Date:** Within 24 hours of task assignment
**Submission Channel:** Jira/Confluence/Email
**Review Process:** Senior QA will review within 48 hours

---

**END OF TASK ASSIGNMENT**

*Note: This document follows standard QA task assignment format used in IT companies. Adjust time estimates and scope based on actual complexity and your experience level.*