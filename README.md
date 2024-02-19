
1.	 Introduction
Testing, in the context of software development, refers to the process of evaluating a system or application to identify any disparities between expected and actual outcomes. The primary goal of testing is to ensure that the software meets specified requirements, functions accurately, and provides a satisfactory user experience. Testing encompasses various activities and techniques designed to uncover defects, faults, or weaknesses in software products.
This documentation outlines the process and results of functional testing conducted on zka-rks.org. Functional testing is essential to ensure that the webpage meets its specified requirements and provides a satisfactory user experience.

2.	 Key Aspects of Testing
There are several aspects related to testing, some of the key ones include:
2.1	Types of Testing
•	Functional Testing: Focuses on verifying that the software operates according to specified requirements. It includes testing the functions, features, and individual interactions within the software.
•	Non-functional Testing: Evaluates aspects of the software beyond its basic functionality, such as performance, usability, security, reliability, and compatibility.
•	Manual Testing: Testing performed by human testers who execute test cases manually without using automation tools.
•	Automated Testing: Testing involves the use of automation tools to execute test cases, compare actual results with expected results, and generate test reports.
2.2	 Testing Levels
•	Unit Testing: Testing of individual components or modules of the software to ensure they function properly in isolation.
•	Integration Testing: Testing of interactions between different modules or components to ensure they function together as expected.
•	System Testing: Testing of the entire system or application as a whole to verify that it meets specified requirements.
•	Acceptance Testing: Testing conducted to determine whether a system meets acceptance criteria and satisfies the needs of stakeholders.
2.3	Testing Processes
•	Test Planning: Defining the objectives of testing, purpose, strategies, and necessary resources for testing.
•	Test Design: Creating test cases, test scenarios, and test data based on requirements and specifications.
•	Test Execution: Execution of test cases, analysis of results, and reporting of defects or issues found during testing.
•	Test Reporting: Documenting test results, generating test reports, and communicating findings to stakeholders.

3.	  Functional Tests
3.1	Test Scenarios
•	Navigation Testing: Verify navigation links and menus across the webpage.
•	Form Submission Testing: Test form submission functionalities, including validation and error handling.
•	Content Display Testing: Ensure all content, images, and multimedia elements load correctly.
•	Search Functionality Testing: Validate search functionalities and search result displays.
•	Language Localization Testing: Test language options and ensure content displays correctly in different languages.

3.2	Test Planning
•	Objectives: Ensure the functionality, usability, and performance of zka-rks.org.
•	Scope: Functional testing of key features and functionalities.
•	Approach: Manual testing by a dedicated testing team.
•	Test Environment: Modern web browsers on different operating systems.
•	Test Schedule: Testing to be conducted over a specified time period.

3.3	Test Strategy
•	Test Objectives: Ensure functionality, usability, security, and performance.
•	Techniques: Black-box testing, exploratory testing, regression testing.
•	Test Coverage: Full coverage of key features and functionalities.
•	Risk Management: Identification and mitigation of potential risks.

3.4	Test Cases
1.	Navigate control in Home Page:
•	Prerequisites: Open the webpage zka-rks.org in a modern web browser.
 Expected: The webpage should open in a web browser without any issues.
Actual: The webpage opened successfully as expected, except the link to the “Databaza e rekomandimeve” wasn’t linked properly and was forwarded to the main page.
2.	Check functionality for search feature
Expected to have a valid search feature, the user should be able to search, and the page should display information related to the search. 
The response was positive, except when searching for a non-existent term, it didn’t indicate that there were no results found.
3.	Contact Form Submission Verification
•	Prerequisites: Ensure a valid email address is available for testing purposes.
•	Test Data Requirement: Valid email addresses for form submission testing.
Expected the page to have a contact page, which would be accessible from the home page.
The contact form is expected to give a warning for unfilled boxes and shouldn’t make it possible to send the form without filling the boxes.
The page does have a contact page, if filled correctly it works properly, but for any other case it does not give any warning, nor stop you from submitting the form.
4.	Document Download Functionality
•	Prerequisites: Open the webpage zka-rks.org in web browser.
•	Test Data Requirement: Document name or type for testing.
Expected download links to work as intended, but it only opened the document in another tab, rather than downloading it.
5.	Responsive Testing
•	Prerequisites: Ensure access to the webpage zka-rks.org.
Expected the webpage to be responsive to any changes in resolution, the page response was successful.
6.	Verify Language Change Functionality
•	Prerequisites: Language options should be clearly displayed and accessible from the webpage.
•	Test Data Requirement: Specific languages or language options to be tested.
Expected the webpage to have the option to change the language of the page, also expected there to be multiple languages.
The page did have an option to change the language of the page, but it didn’t cover the translation of everything.
7.	Verify Video Display
•	Prerequisites: Ensure availability of video elements on the webpage.
•	Test Data Requirement: Specific video elements or test videos required for testing.
Expected the page to have playable videos, only one video to be played at once, be able to control the video (play, pause, skip, forward, backward).
The page did have playable videos, but it only had 3 distinct videos, where 1 of them was repeated 15 times, and the user could play multiple videos at once.


3.5	Report
Bug: 
•	Test Case 1: Step 4
•	Test Case 2: Step 4
•	Test Case 3: Step 2-6
•	Test Case 4: Step 2, Step 4
•	Test Case 5: 0
•	Test Case 6: 0
•	Test Case 7: Step 2
Error:
•	Test Case 1: 0
•	Test Case 2: 0
•	Test Case 3: Step 7
•	Test Case 4: 0
•	Test Case 5: 0
•	Test Case 6: Step 4
•	Test Case 7: 0 
Failure:
•	Test Case 1: 0
•	Test Case 2: 0
•	Test Case 3: 0
•	Test Case 4: Step 3
•	Test Case 5: 0
•	Test Case 6: Step 6
•	Test Case 7: Step 5
 
4.	 Non-functional Tests
Incorporated within our non-functional testing phase are comprehensive evaluations, including load, stress, and accessibility tests. These assessments are conducted to guarantee system stability, optimize performance, and enhance overall inclusivity.
4.1.	Load Testing
Load testing has been conducted in our project to assess the performance and capacity of the web page under various loads. The main goal is to identify system limits and improve overall performance under intensive loads. For this testing process, we chose JMeter for its ability to simulate high loads, monitor performance, and provide detailed performance metrics.
Configuration Steps:
	Number of Users: We started with a group of 100 users and gradually increased to 2000.
	Think Time: We used a 1-second think time to simulate real user behavior.
After conducting the tests, after surpassing 1500 users, we noticed that the web page no longer accepted more users and exhibited significant signs of slowdown.

![image](https://github.com/ermallimaj/functional-and-non-functional-testing-ZKA-webpage/assets/121945435/3300338e-73cb-4fb6-b008-df434d0d38b5)
                                             Figure 1. JMeter Load Testing Summary Report

4.2.	Stress Testing
In the stress testing phase using JMeter, our objective was to evaluate the system's performance under varying loads to identify its capacity limits and potential points of failure. Throughout this testing, we systematically increased the number of simulated users to assess how the system responds under stress conditions.

Stress Testing Results:
The system demonstrated robust performance up to a load of 1,500 users, exceeding expectations in terms of response time and transaction success rate. However, as the user load continued to increase, a degradation in system performance was observed, with the system accepting a maximum of only 262 users.
![image](https://github.com/ermallimaj/functional-and-non-functional-testing-ZKA-webpage/assets/121945435/03f3c6bf-4966-483a-8ac4-8f2a7e4872aa)
                                             Figure 2. JMeter Stress Testing Result in Table
4.3.	Accessibility Testing
We tested the website to see how easy it is for everyone to use. We used a tool called ax DevTools to find any issues in different parts of the site, such as menus and forms. We focused on things like how pictures are described, whether interactive parts are easy to see, and special codes used for certain elements. The aim was to identify areas where the website might need improvement to follow the rules that make websites accessible, ensuring that everyone can use it without any problems.
![image](https://github.com/ermallimaj/functional-and-non-functional-testing-ZKA-webpage/assets/121945435/e6ad3739-b8d1-46ab-878f-bfe1740ac31a)
                                             Figure 4. Total issues found with Ax DevTools

![image](https://github.com/ermallimaj/functional-and-non-functional-testing-ZKA-webpage/assets/121945435/26f26c94-193c-47a8-aa56-3ee78915934f)
                                             Figure 5. Identified specific issues using Ax DevTools
                                             
Contributors:
1. Agnesa Jashanica
2. Arijesa Muja
3. Eriona Mustafa
4. Erisa Cervadiku
5. Ermal Limaj
