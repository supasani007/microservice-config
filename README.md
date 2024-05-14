- **Project Name**: AutoDeskProject

- **Brief project description**:
   This project contains automated end to end test suites that tests the functionality of the calculator component on Google.
   Theses tests are written considering that the calculator only has the buttons **0123456789.=+-×÷AC/CE** using the page factory design
   pattern by using tools such has Java, JUnit, Selenium.

- **Table of Contents**:
   1. [Features](#Features)
   2. [Installation](#Installation)
   3. [Usage](#Usage)
  
- <a name="Features">Features</a>:
    1. This project includes tests for different operations that can be performed on a google calculator which includes:

        A. Addition: basic addition, addition with zero, add positive and negative integer, add 2 negative integers, add 2 decimal numbers, add with result exceeding the display limit, add after clearing calculator
        
        B. Subtraction: basic subtraction, subtraction with zero, subtract 2 negative integers, subtract 2 decimal numbers, subtract with result exceeding the display limit, subtract after clearing calculator
        
        C. Multiplication: basic multiplication, multiply with zero, multiply with negative integers, multiply 2 decimal numbers, multiply with result exceeding the display limit, multiply after clearing calculator
        
        D. Division: basic division, division with one, division by zero, divide positive and negative integers, divide 2 negative integers, divide 2 decimal numbers, divide with result exceeding the display limit, divide after clearing calculator
        
        E. Edge cases: test error expression, test for very large number, test for extreme negative number, test for very small number
        
        F. Test combination: test multiple operations
       
    3. Test retry feature which retries every test 2 times before considering it as a failure.
    4. Takes screenshots of the failing tests and stores them in the screenshot directory.
    5. Logs the test results and also which method has been executed and store the logs in logs/app.log file.


- <a name="Installation">Installation</a>:
    1. Download the project
    2. Open it using any of the IDEs say IntelliJ
    3. Make sure to have the latest chrome and firefox version running locally as test runs on those
    4. Right click on pom.xml and reload project to install all the dependencies needed to the tests
    5. Download latest chrome driver from https://googlechromelabs.github.io/chrome-for-testing/#stable
    6. Download latest firefox driver from https://github.com/mozilla/geckodriver/releases

- <a name="Usage">Usage</a>: Follow these steps on how to run the tests individually and as a group:
    1. Right click on the any test class under com.calculator.tests to run an individual test class or test case
    2. Right click on the directory com.calculator.tests to run all tests together
    3. Right click on the testsuite classes under the com.calculator.testsuites directory to run different test suites
    4. Uncomment {"firefox"} line in BaseClass file to run the tests on both chrome and firefox


