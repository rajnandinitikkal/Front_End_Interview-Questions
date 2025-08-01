### 1) Test Levels :-> 
   - Component/Unit
   - Component Integration
   - System
   - System Integration
   - UAT

### 2) Diff Between Regression and Retesting 
   
   - Regression Testing: Testing the unchanged parts of the application to ensure that recent changes haven’t broken existing functionality.

   - Retesting: Testing the same defect after it has been fixed to ensure it is resolved.

### 3) What are the most important things you have to consider when you're writing tset cases ? 

✅ 1. Clear Test Case Objectives
Define what functionality you're testing and why.

Each test case should have a clear purpose.
✅ 2. Good Test Case Structure
Include:
- Test Case ID
- Title/Name
- Preconditions/ Assumptions
- Test Criteria
- Test Steps
- Expected Result
- Actual Result (during execution)
- Pass/Fail status

✅ 3. Test Coverage
Ensure you cover all requirements and scenarios: positive, negative, boundary, edge cases, etc.

✅ 4. Traceability to Requirements
Each test case should be mapped to a specific requirement to ensure all features are tested.

✅ 5. Reusability and Maintainability
Write modular and reusable test steps to save time when maintaining tests.

✅ 6. Clarity and Simplicity
Use clear, simple language so anyone (even non-testers) can understand and execute it.

✅ 7. Avoid Assumptions
Be explicit about inputs, environment, and data—don't assume any conditions.

✅ 8. Test Data Preparation
Ensure test data is available and clearly defined for each case.

✅ 9. Priority and Severity
Identify which test cases are critical and should be executed first.

✅ 10. Review and Peer Validation
Get test cases reviewed by peers or leads to catch gaps or errors.

### 4) Diff between White Box and Black box 

✅ White Box Testing
Tests internal code and logic
Requires programming knowledge
Done by developers

✅ Black Box Testing
Tests functionality without looking at code
Based on requirements
Done by testers/QA

### 5) What is Selenium
- Selenium is a free, open-source tool used for automating web browsers.

🔹 Key Points:
It is mainly used for automated testing of web applications.
Supports multiple browsers (Chrome, Firefox, Safari, Edge).
Works with multiple programming languages (Java, Python, C#, JavaScript, etc.).
Can be integrated with tools like TestNG, JUnit, Maven, Jenkins for advanced testing workflows.

🧪 Common Components:
Selenium WebDriver – Automates browser actions.
Selenium IDE – A Chrome/Firefox plugin for record-and-playback testing.
Selenium Grid – Runs tests on multiple machines/browsers in parallel.

### 6) Tools
- JIRA
- Bugzilla
- Recordil
- Trello
- Postman
- Jmeter

### 7) Differnt Types of Testing

✅ 1. Functional Testing
Tests what the system does.

Unit Testing – Tests individual units/components (done by developers).

Integration Testing – Tests the interaction between integrated units/modules.

System Testing – Tests the entire application as a whole.

Sanity Testing – Quick check to ensure basic functionality works.

Smoke Testing – Basic test to ensure the build is stable.

Regression Testing – Checks existing functionality after code changes.

User Acceptance Testing (UAT) – Final testing by end users before release.

✅ 2. Non-Functional Testing
Tests how the system performs. Tool used for Non-functional testing is  "JMETER"

Performance Testing – Checks speed, responsiveness.

Load Testing – Tests system under expected user load.

Stress Testing – Tests system under extreme load.

Security Testing – Ensures data protection and access control.

Usability Testing – Tests user experience and interface.

Compatibility Testing – Ensures the app works on different devices, OS, browsers.

✅ 3. Maintenance Testing
Re-testing – Verifying bug fixes.

Regression Testing – Re-checking for side effects after changes.

✅ 4. Other Specialized Testing
Exploratory Testing – Simultaneously learning and testing the application.

Ad-hoc Testing – Informal testing without a test plan.

Alpha Testing – Done by internal users before release.

Beta Testing – Done by external users after alpha testing.




