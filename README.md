- **Project Name**: AutoDeskProject

- **Brief project description**:
   This project contains automated end to end test suites that tests the functionality of the calculator component on Google.
   Theses tests are written considering that the calculator only has the buttons **0123456789.=+-×÷AC/CE** using the page factory design
   pattern by using tools such has Java, JUnit, Selenium.

- **Table of Contents**:
   1. [Features](#Features)
   2. [Installation](#Installation)
   3. [Project Structure](#ProjectStructure)
   4. [Usage](#Usage)
   5. [Todo](#Todo)
  
- <a name="Features">Features</a>:
    1. This project includes tests for different operations that can be performed on a google calculator which includes:

        A. Addition: basic addition, addition with zero, add positive and negative integer, add 2 negative integers, add 2 decimal numbers, add with result exceeding the display limit, add after clearing calculator
        
        B. Subtraction: basic subtraction, subtraction with zero, subtract 2 negative integers, subtract 2 decimal numbers, subtract with result exceeding the display limit, subtract after clearing calculator
        
        C. Multiplication: basic multiplication, multiply with zero, multiply with negative integers, multiply 2 decimal numbers, multiply with result exceeding the display limit, multiply after clearing calculator
        
        D. Division: basic division, division with one, division by zero, divide positive and negative integers, divide 2 negative integers, divide 2 decimal numbers, divide with result exceeding the display limit, divide after clearing calculator
        
        E. Edge cases: test error expression, test for very large number, test for extreme negative number, test for very small number
        
        F. Test combination: test multiple operations
       
    3. Test retry feature which retries every test 2 times before considering it as a failure.
    4. Logs the test results and also which method has been executed and store the logs in logs/app.log file.
    5. Takes screenshots of the failing tests and stores them in the screenshot directory.


- <a name="Installation">Download and Installation</a>:
    1. Download the project
    2. Open it using any of the IDEs say IntelliJ
    3. Make sure to have the latest chrome and firefox version running locally as test runs on those
    4. Right click on pom.xml and reload project to install all the dependencies needed to the tests
    5. Download latest chrome driver from https://googlechromelabs.github.io/chrome-for-testing/#stable
    6. Download latest firefox driver from https://github.com/mozilla/geckodriver/releases

- <a name="ProjectStructure">Project Structure</a>:
    1. Configuration directory has all the hardcoded values in the configuration.properties file
    2. Driver has all the drivers used for this project which includes chrome and firefox drivers
    3. Logs stores all the logs generated in the project in the app.log file
    4. test/java/com/calculator:

        A. Interfaces: includes all the interfaces to run different test suites 

        B. PageObject: includes page object class for calcualtor with all the methods defined for different operations and 
                       basetest class to initiate drivers, set up the browser and setup and teardown methods
        
        C. Tests: includes classes for all tests defined the feature section above
        
        D. TestSuites: currently has 2 test suites ComplexTestSuite: with tests categorized as complex and SmokeTestSuite: with tests categorized as smoke or happy path tests in the test classes
        
        E. Utilities: includes configreader: to read the configuration file values, 
                          retrytestwatcher: to retry test a given number of times,
                          screenshotonfailure: take screenshot on test failure 


- <a name="Usage">Usage</a>: Follow these steps on how to run the tests individually and as a group:
    1. Right click on the any test class under com.calculator.tests to run an individual test class or test case
    2. Right click on the directory com.calculator.tests to run all tests together
    3. Right click on the testsuite classes under the com.calculator.testsuites directory to run different test suites
    4. Uncomment {"firefox"} line in BaseClass file to run the tests on both chrome and firefox

- <a name="Todo">Todo</a>:
    1. Add a section for code coverage with test success and failures over a period of time
    2. Add more test suites under the com.calculator.testsuites directory based on the requirement
    3. Add utility classes for test data driven testing 
    4. Add support for more drivers such as IE, Edge, etc. 
    5. Add support for sauce labs so as to enable tests to run on a remote machine with multiple browser and OS combination




