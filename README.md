# Sample Agile Test Strategy
This is a sample test strategy document used to list practices and a structure that teams can use to improve the testing approach


***
### Purpose
The purpose of the document is to create a shared understanding of the overall goals, approach, tools and timings of testing activities that can be followed to ensure delivery of the product with predictable bheviour, performance and quality.

The test strategy guides us through common obstacles with a clear view of how to evaluate the system. Testing starts with exploration of the user stores and what the stakeholders really wants by elabroating the user stories from different perspectives.


***
### Goal

To continuously deliver quality software that meets customer's requirements by means of quick feedback and defect prevention.

Achieved by:

 - Having layers of tests to catpture bugs/defects early in the development life cycle
 - Reduce time taken for regression

***
### Principles

***
### Testing Approach

Having layers of tests essentially act as a risk filter that tries to filters anomalies at verious levels.

#### Test Pyramid

 The Testing Pryamid is a framework that helps the engineering team create high-quality software. It helps the team reduce time in identifying breaking changes and be more confident in introducing code changes.

The bulk of your tests are unit tests at the bottom of the pyramid. As you move up the pyramid, your tests gets larger, but at the same time the number of tests (the width of your pyramid) gets smaller.

As a good first guess, it is often suggested a 70/20/10 split: 70% unit tests, 20% integration tests, and 10% end-to-end tests. The exact mix differs for every team, but in general, it should retain that pyramid shape.

   **Operation level**
              
  - Level 1 : [Unit tests ](#unit_tests)
  - Level 2 : [Integration tests/Contract tests](#integration_tests)
  - Level 3 : [End-to-End test](#e2e_tests)
  - Level 4 : [Manual Exploratory Testing](#exploratory_tests)


    
 ![Testing Pyramid](https://d2h1nbmw1jjnl.cloudfront.net/ckeditor/pictures/data/000/000/158/content/typical_pyramid-1024x938.jpg)   
**The Testing Pyramid**
               [Image source](https://www.ministryoftesting.com/dojo/lessons/the-mobile-test-pyramid)
              

<a name="unit_tests"></a>
#### Unit Tests

Unit tests are to provide confidence about specific implementations of logic that could be harder to test at the service level, or to verify specific exceptional behaviour that is difficult or time consuming to produce at the service level.

Service Level Tests

These tests bring up the service and any of it's managed dependencies to simulate a complete service. Any external dependencies are mocked/simulated so that service behaviour can be verified. The focus of this level of test is to ensure the service behaviour is correct. 

<a name="integration_tests"></a>
#### Integration Tests
Integration test is to test whether many separately developed modules work together as expected. It was performed by activating many modules and running higher level tests against all of them to ensure they operated together. The pupose of integration test is to ensure:

- Detecting defects early
- Earlier feedback on the acceptability of the individual module will be made available
- Scheduling of defect fixes is flexible
- Correct data flow
- Correct control flow
- Correct with software requirements

**Different test approaches and tools that are used for different type of integration test**

- Integration tests between UI components in the same and different modules

   [Tools](#tools): Cypress, Selenium Web Driver

- Functional API Test

   [Tools](#tools): PostMan, RestSharp, RestAssured etc.
  
- Test integration between UI components and APIs (mocked)

   [Tools](#tools): Cypress, Selenium Web Driver 4

<a name="e2e_tests"></a>
#### End-to-End Test

End-to-end testing is a technique that tests the entire software product from beginning to end to ensure the application flow behaves as expected. It defines the product’s system dependencies and ensures all integrated pieces work together as expected.

[Tools](#tools): Selenium Web Driver, Cypress, Appium(for mobile)

<a name="exploratory_tests"></a>
#### Exploratory Testing

Exploratory testing is a testing technique where an individual explores the system in real-time using their experience and practical thinking. It is a simultaneous learning, test design, and test execution process.



***
### Tools
<a name="tools"></a>

 - [Cypress](https://www.cypress.io/)
 - [Selenium Web Driver](https://www.selenium.dev/documentation/webdriver/)
 - [Postman](https://www.postman.com/)
 - [Jmeter](https://jmeter.apache.org/)


***
### Test Deliverables

***
### Assumptions, Risks and Dependencies
| Assumption      | Impact of incorrect Assumptions |
| ----------- | ----------- |
| Assumption 1      | :skull:       |
| Assumption 2  | :skull:        |
