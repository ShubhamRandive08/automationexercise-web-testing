# **MANUAL TESTING TASK ASSIGNMENT**

##### **Project:** `Automation Exercise E-commerce Platform`
##### **Module:** `Login Page Testing`
##### **Document ID:** `QA-TASK-AUTOEX-LOGIN-001`
##### **Priority:** `High`
##### **Assigned To:** `Shubham Randive`
##### **Estimated Effort:** `3-4 hours`

---

## **1. TASK OVERVIEW**
You have been assigned to perform comprehensive manual testing on the Login page of the Automation Exercise e-commerce platform. Based on the provided UI screenshots, you are required to design, execute, and document test scenarios covering functional, UI/UX, security, and usability aspects of the login functionality.

## **2. TEST OBJECTIVE**
Validate that the Login page functions correctly according to specifications, provides secure authentication, offers intuitive user experience, and handles all possible user interactions appropriately for both new and existing users.

## **3. SCOPE OF TESTING**
**In-Scope:** Login form functionality (via "Signup / Login" button), UI/UX elements verification, Input field validations (Email & Password), Authentication logic (New User vs Existing User), Navigation elements, Error handling mechanisms, Security aspects, Responsive behavior.

**Out-of-Scope:** Backend API testing, Performance/Load testing, Database validation, Third-party integrations, Mobile application testing, Product listing/cart functionality.

## **4. TEST ENVIRONMENT DETAILS**
- **Base URL:** https://automationexercise.com
- **Login Page URL:** https://automationexercise.com/login
- **Browser Compatibility:** Chrome v115+, Firefox v110+, Edge v115+
- **Screen Resolutions:** 1920x1080, 1366x768, 1536x864, 375x667

## **5. MANDATORY TEST SCENARIOS**

### **SCENARIO 1: NAVIGATION TO LOGIN PAGE**
**Objective:** Verify proper navigation from homepage to login page.

1. Navigate from homepage to login page via "Signup / Login" button
2. Verify login page URL is correct
3. Verify page title contains "Automation Exercise"
4. Verify breadcrumb navigation (if present)
5. Verify browser back button returns to homepage

### **SCENARIO 2: UI ELEMENTS VERIFICATION**
**Objective:** Verify all UI elements are present and properly aligned.

1. Verify "Login to your account" heading is displayed
2. Verify "New User Signup!" section is present
3. Verify email address field with label
4. Verify password field with label
5. Verify "Login" button is present and enabled
6. Verify "Signup" button for new users
7. Verify header navigation elements (Home, Products, Cart, Contact us)
8. Check all text spelling and grammar
9. Verify font consistency across page
10. Verify field placeholder text (if any)

### **SCENARIO 3: FUNCTIONAL VALIDATION - POSITIVE FLOW**
**Objective:** Validate successful login with valid credentials.

1. Login with valid registered email and correct password
2. Verify successful redirection after login
3. Verify "Logged in as [username]" appears in header
4. Verify session persistence across page refresh
5. Verify "Logout" option replaces "Signup / Login"
6. Verify browser back button behavior after login
7. Verify direct access to protected pages after login

### **SCENARIO 4: FUNCTIONAL VALIDATION - NEGATIVE FLOW**
**Objective:** Validate error handling for invalid login attempts.

1. Login with valid email but incorrect password
2. Login with invalid email format
3. Login with unregistered email address
4. Login with empty email field
5. Login with empty password field
6. Login with both fields empty
7. Verify appropriate error messages display
8. Verify error message disappears on field focus
9. Test maximum login attempts limitation
10. Verify account lockout message (if applicable)

### **SCENARIO 5: INPUT FIELD VALIDATIONS**
**Objective:** Validate input field constraints and behaviors.

**Email Field Tests:**
1. Verify valid email format acceptance
2. Verify invalid email format rejection
3. Verify maximum character limit
4. Verify copy-paste functionality
5. Verify space character handling
6. Verify case sensitivity (if applicable)
7. Verify autocomplete behavior

**Password Field Tests:**
1. Verify password masking (asterisks/dots)
2. Verify show/hide password toggle (if available)
3. Verify minimum password length validation
4. Verify maximum password length validation
5. Verify special character acceptance
6. Verify copy prevention (if security feature)
7. Verify password strength indicator (if present)

### **SCENARIO 6: NEW USER SIGNUP SECTION**
**Objective:** Validate new user registration functionality.

1. Verify "New User Signup!" section visibility
2. Verify name field presence and functionality
3. Verify signup email field functionality
4. Verify "Signup" button functionality
5. Verify successful new user registration
6. Verify duplicate email registration handling
7. Verify validation messages for empty fields
8. Verify redirect after successful signup

### **SCENARIO 7: SECURITY TESTING**
**Objective:** Validate security aspects of the login mechanism.

1. Verify HTTPS protocol usage
2. Verify password transmission encryption
3. Test SQL injection attempts: `' OR '1'='1`
4. Test XSS payloads: `<script>alert('test')</script>`
5. Verify browser password saving prompt
6. Verify session timeout after inactivity
7. Test concurrent login restrictions
8. Verify no sensitive data in page source
9. Verify CAPTCHA implementation (if present)
10. Verify CSRF token implementation

### **SCENARIO 8: NAVIGATION & LINKS**
**Objective:** Validate all navigation elements and links.

1. Verify "Home" link functionality from header
2. Verify "Products" link functionality
3. Verify "Cart" link functionality
4. Verify "Contact us" link functionality
5. Verify "Test Cases" link functionality
6. Verify "API Testing" link functionality
7. Verify "Video Tutorials" link functionality
8. Verify browser refresh during login process
9. Verify navigation with incomplete login form
10. Verify all external links open correctly

### **SCENARIO 9: USABILITY & ACCESSIBILITY**
**Objective:** Validate user-friendly experience and accessibility.

1. Verify tab navigation order: Email → Password → Login
2. Verify Enter key submits login form
3. Verify field auto-focus on page load
4. Verify keyboard-only navigation
5. Verify screen reader compatibility
6. Verify color contrast ratios (WCAG compliance)
7. Verify responsive design on different screen sizes
8. Verify error message clarity and helpfulness
9. Verify form labels are properly associated
10. Verify focus indicators on interactive elements

### **SCENARIO 10: EDGE CASES & EXPLORATORY**
**Objective:** Identify unexpected behaviors and edge conditions.

1. Login with extremely long email address
2. Login with extremely long password
3. Submit form multiple times quickly (double-click)
4. Login during network interruption
5. Change URL parameters during login process
6. Test with browser zoom (80%, 100%, 125%, 150%)
7. Test with browser developer tools open
8. Test with ad-blockers enabled
9. Test with cookies disabled
10. Test with JavaScript disabled
11. Test across different time zones
12. Test with special characters in credentials

### **SCENARIO 11: BROWSER COMPATIBILITY**
**Objective:** Verify consistent behavior across browsers.

1. Test login functionality on Chrome latest
2. Test login functionality on Firefox latest
3. Test login functionality on Edge latest
4. Verify responsive design across browsers
5. Verify error message display consistency
6. Verify form submission behavior consistency
7. Verify session management across browsers
8. Verify cookie handling consistency

### **SCENARIO 12: SESSION MANAGEMENT**
**Objective:** Validate proper session handling.

1. Verify login session persists across tabs
2. Verify login session persists after browser restart
3. Verify logout clears session properly
4. Verify session timeout after inactivity
5. Verify concurrent session handling
6. Verify "Remember me" functionality (if present)
7. Verify session cookie attributes (HttpOnly, Secure)
8. Verify forced logout on password change

## **6. DELIVERABLES REQUIREMENTS**
**Mandatory Deliverables:**
1. Test Execution Report (Excel/Google Sheets format)
2. Defect/Bug Report (For each failure found)
3. Test Summary Report (Overall execution summary)

**Format Specifications:**
- Use test case naming convention: `AUTOEX-LOGIN-TC-001`
- Save screenshots as: `AUTOEX-LOGIN-SCR-YYYYMMDD-HHMMSS.png`
- Submit all documents in: `AUTOEX-LOGIN-REPORT-YYYYMMDD.zip`

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
- Test data is available or can be created
- No major changes to UI during testing period

**Risks:**
- Environment downtime may impact testing
- Test data issues may block scenarios
- Browser compatibility issues may occur

**Dependencies:**
- Access to test environment
- Availability of test accounts
- Functional requirements document

**Escalation Point:** Team Lead/QA Manager for any blocking issues

## **9. SUBMISSION DETAILS**
**Due Date:** Within 24 hours of task assignment
**Submission Channel:** Jira/Confluence/Email
**Review Process:** Senior QA will review within 48 hours

---

**END OF TASK ASSIGNMENT**

*Note: This document follows standard QA task assignment format used in IT companies. Adjust time estimates and scope based on actual complexity and your experience level.*