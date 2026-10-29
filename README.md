# SoapBox CI/CD

A software quality assurance and deployment project focused on automated testing, continuous integration, and reliable account workflows for a Django-based web application.

## Tech Stack

- Python
- Django
- GitLab CI/CD
- Django Test Framework
- Selenium
- Chrome / ChromeDriver
- HTML
- SQLite

## Project Focus

The project emphasizes software quality through automated unit testing, browser-based functional testing, and continuous integration. Testing centers on critical account functionality such as registration, authentication, access control, and logout behavior.

## CI Pipeline

The GitLab CI/CD pipeline uses a Python container, installs the required Django environment, and automatically runs the application test suite on pipeline execution.

```text
Code Change
    ↓
GitLab CI Pipeline
    ↓
Python / Django Environment
    ↓
Automated Test Execution
    ↓
Pass / Fail Result
```

The pipeline executes the Django test suite with:

```text
python manage.py test app1 -v 2
```

## Automated Test Coverage

Seven automated Django tests validate core user and authentication behavior, including:

- Successful account registration
- Password mismatch handling
- Successful login
- Failed login
- Authenticated home-page access
- Unauthenticated home-page access
- Logout behavior

The documented pipeline result completed all seven tests successfully with an `OK` result and successful job completion.

## Browser Automation

Selenium with Python and Chrome was used for automated browser testing of registration and login workflows. The browser automation uses reusable page-element locators and verifies expected user-facing behavior through end-to-end interaction with the application.

## Quality Engineering Practices

The project demonstrates:

- Automated regression testing
- Positive and negative test scenarios
- Authentication and access-control validation
- Continuous integration
- Browser-based functional testing
- Repeatable test execution
- Pipeline-based quality gates

## Source Code

The original implementation is maintained in a private academic repository. Source access can be provided for professional review upon request.

## Author

**Nicholas Cornes**  
B.S. Software Engineering
