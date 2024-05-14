- **Project Name**: AutoDeskProject

- **Brief project description**:
   This project contains automated end to end test suites that tests the functionality of the calculator component on Google.
   Theses tests are written considering that the calculator only has the buttons 0123456789.=+-×÷AC/CE using the page factory design
   pattern by using tools such has Java, JUnit, Selenium.

- **Table of Contents**:
   A. [Features](#Features)
   B. [Installation](#Installation)
  
- <a name="Features">Features</a>
    1. This project includes tests for different operations that can be performed on a google calculator which includes:
        A. Addition
        B. Subtraction
        C. Multiplication
        D. Division
        E. Edge cases
    2. It has a test retry feature which retries every test 2 times before considering it as a failure.
    3. It takes screenshots of the failing tests and stores them in the screenshot directory.
    4. It logs the test results and also which method has been executed.


- <a name="Installation">Installation</a>
    1. Download the project
    2. Open it using any of the IDEs say IntelliJ
    3. Make sure to have the latest chrome and firefox version running locally as test runs on those
    4. Right click on pom.xml and reload project to install all the dependencies needed to the tests
    5. Download latest chrome driver from https://googlechromelabs.github.io/chrome-for-testing/#stable
    6. Download latest firefox driver from https://github.com/mozilla/geckodriver/releases


- **Usage**: Follow these steps on how to run the tests individually and as a group
    1. Right click on the any test class under com.calculator.tests to run an individual test class or test case
    2. Right click on the directory com.calculator.tests to run all tests together
    3. Right click on the testsuite classes under the com.calculator.testsuites directory to run different test suites

- **Configuration**: Describe any configuration options or settings that users may need to adjust.
- **Contributing**: Provide guidelines for contributing to the project.


