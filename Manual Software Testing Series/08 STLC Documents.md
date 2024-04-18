

# Test Plan Contents
- a document that describe the test scope, test strategy, objectives, schedule, deliverables, and resources required to perform testing for a software product. 
- before testing, we will do planning 

Test Plan Template Contents:
- overview - what is the project why we are preparing the test document.
- scope - what to test and not to test - it will be based on the customer document.
	- inclusions
	- test environments
	- exclusions
- test strategy - type of testing to conduct - smoke, sanity, regression, etc. Manual or Automated.
- defect reporting procedure - how we are going to report the bugs
- roles/responsibilities - specify test engineer, test lead, project manager.
- test schedule - specify the date and action will do 
- test deliverables - every phase of testing we will deliver some kind of documents such as test plan, test cases, defect report, test execution, etc., responsibility of management
- pricing - responsibility of management
- entry and exit criteria - when to start and exit the testing 
- suspension and resumption criteria - sometime we will stop testing because of some error, and after get fixed, it will resume immediately. Specify which cases will stop and resume testing.
- tools - excel, word, manual testing or automated testing, bug tracking, test management.
- risk and mitigations - plan if people accident and mitigations.
- approvals - when do we need to get approval, who will approve the test case - when do we need to get approval, who will approve the test case


# Use Case, Test Scenario, Test Case

## Use Case
- describes the requirement.
- contains three(3) items:
	- actor - which is the user, can be a single person or a group of people, interacting with a process.
	- action - which is to reach the final outcome. 
	- goa/outcome - which is the successful user outcome. 
- product manager/owner will write the use case.

## Test Scenario
- a possible area to be tested (what to test)	


## Test Case
- step by step actions to be performed to validate functionality of AUT (Application Under Test) (How to test)
- test case contains test steps, expected result and actual result.


## Use Case vs Test Case
- Use case - describes the functional requirement, prepared by Business Analyst (BA).

- Test case - describes test steps/procedure, prepared by Test Engineer(TE). Prepared based on Use Case.



## Test Scenario vs Test Case
- Test Scenario is "What to be tested".
- Test Case is "How to be tested".

Example:
	Test Scenario: Checking the functionality of Login Button.
		TC1: Click the button without entering username and password.
		TC2: Click the button only entering username.
		TC3: Click the button while entering wrong username and password.



# Test Suite
- a group of test cases which belongs to the same category.

![[Test Suite.png]]



# Test Case
- a set of actions executed to validate particular feature or functionality of your software application.

Test Case Contents:
- Test Case ID - every test case should be unique using identification(ID)
- Test Case Title - one or two lines, refers to test case
- Description - three to four lines about the test case
- Pre-condition - before executing the test case, what are requirements should be satisfied. 
- Priority (P0, P1, P2, P3) - order - in which order we will execute the test case. What should be first to execute? P0 - Smoke testing, P1 - Regression Testing, P2 - Functional Testing, P3 - UI Related Testing.
- Requirement ID - which requirement we are writing the test cases. 
- Steps/Actions - ex. go to this, input this, click this, etc.
- Expected Result - what should output based on the requirements document.
- Actual Result - what is the actual output of the test.
- Test Data - what are the inputs or data of the test.



# Test Case Template
![[Test case template.png]]




# Requirement Traceability Matrix (RTM)
- RTM describes the mapping of Requirement's with the Test cases. 
- main purpose is to see that all test cases are covered so that no functionality should miss while doing software testing.

RTM - Parameters Include:
- Requirement ID
- Requirement Description
- Test case IDs

![[Requirement Traceability Matrix (RTM).png]]





# Test Environment
- is a platform specially build for test case execution on the software product.
- it is created by integrating the required software and hardware along with proper network configurations.
 - simulates production/real time environment.
- also called "Test Bed".



# Test Execution
- during this phase, test team will carry out the testing based on the test plans and the test cases prepared.
- Entry Criteria: Test cases, Test Data, and Test Plan
- Activities:
	- test cases are executed based on the test planning.
	- status of test cases are marked, like Passed, Failed, Blocked, Run, and others.
	- documentation of test results and log defects for failed cases is done.
	- all the blocked and failed test cases are assigned bug ids.
	- retesting once the defect is fixed.
	- defects are tracked til closure.



# Guidelines for Test Execution
- the build being deployed to the QA environment is the most important part of the test execution cycle.
- test execution is done in Quality Assurance (QA) environment.
- test execution happens in multiple cycles.
- test execution phase consists executing the test cases + test scripts (if automation).



# Defects/Bugs
- any mismatched functionality found in an application is called as Defect/Bug/Issue.
- during Test Execution, Test Engineers are reporting mismatches as defects to developers through templates or using tools.
- Defect Reporting Tools:
	- clear quest
	- devtrack
	- jira
	- quality center
	- bug jilla
	- etc.


# Defect Report Contents
- Defect ID - unique identification number for the defect.
- Defect Description - detailed description of the defect including information about the module in which defect was found.
- Version - version of the application in which the defect was found.
- Steps - detailed steps along with screenshots with which the developer can reproduce the defects.
- Date Raised - date when the defect is raise.
- Reference - where you provide reference to the documents like requirements, design, architecture or may be even screenshots of the error to help understand the defect.
- Detected by - name/id of the tester who raised the defect.
- Status - status of the defect, more on this later. This will changed if the bug is fixed or not.
- Fixed by - name/id of the developer who fixed it.
- Date closed - date when the defect is closed.
- Severity - describes the impact of the defect on the application.
- Priority - which is related to defect fixing urgency. Severity Priority could be High/Medium/Low based on the impact urgency at which the defect should be fixed respectively.




# Defect Classification
- tester responsibility

Severity:
- Blocker
- Critical
- Major
- Minor

Priority:
- P1
- P2
- P3
 
![[Defect Classification.png]]

## -Defect Severity-
- severity describes the seriousness of defect and how much impact on Business workflow.

Defect can be categorized into four class:
- Blocker(Show stopper): This defect indicates nothing can proceed further.
	- Ex. Application crashed, Login not worked
- Critical - the main/basic functionality is not working. Customer business workflow is broken. They cannot proceed further.
	- ex. 1: fund transfer is not working in net banking.
	- ex. 2: ordering product in ecommerce application is not working.
- Major - it cause some undesirable behavior, but the feature/application is still functional. 
	- ex. 1: after sending email, there is no confirmation message.
	- ex. 2: after booking cab, there is no confirmation.
- Minor - it won't cause any major break-down of the system.
	- ex. 1: look and feel issues, spellings, alignments.





## -Defect Priority-
- describes the importance of defect
- states the order which a defect should be fixed.
- defect priority can be categorized into three(3) class:
	- P0 (High) - the defect must be resolved immediately as it affects the system severely and cannot be used until it is fixed.
	- P1 (Medium) - it can wait until a new versions/build is created.
	- P2 (Low) - developer can fix it in later releases.

note: whenever we report defect to developer, we need to provide severity and priority. Priority can be changed based on product owner or Business Analyst. 


# Examples of Severity and Priority

![[severity and priority example.png]]


![[severity and priority example 2.png]]



# Defect Resolution
- after receiving the defect report from the testing team, development team conduct a review meeting to fix defects. Then they send a Resolution Type to the testing team for further communication.

Resolution Types:
- Accept
- Reject 
- Duplicate
- Enhancement
- Need more information
- Not Reproducible
- Fixed
- As Designed






























