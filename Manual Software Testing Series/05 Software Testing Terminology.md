# Regression Testing
- testing conducts on modified build to make sure there will not be impact on existing functionality because of changes like adding/deleting/modifying features.

#### --Unit Regression Testing
- testing only the changes/modifications done by the developer
- test the specific bug that have been reported 

#### --Regional Regression Testing
- testing the modified module along with the impacted modules
- impact analysis meeting conducts to identify impacted modules with QA and Dev


#### --Full Regression 
- testing the main feature and remaining part of the application 
- Ex. Dev has done changes in many modules, instead of identifying impacted modules, we perform one round of full regression



# Re-testing
- conducted after tester reported a bug to developer then verify if the bug is fixed
- test only the bug that has been reported previously if it is fixed
- whenever developer fixed a bug, tester will test the bug fix is called Re-testing
- to ensure that the defects were found and posted in the earlier build were fixed or not in the current build

# Smoke vs Sanity Testing
- these testing come after build release
- if the smoke and sanity testing is successful then the build is accepted,
- sanity testing is part of regression testing
- in every cycle, tester will conduct smoke and sanity testing

| Smoke Testing                                                                                            | Sanity Testing                                                                                                                 |
| -------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| smoke testing is done to make sure the build we received from development team is testable/stable or not | sanity testing is done during the release phase to check for the main functionalities of the application without going deeper. |
| smoke testing is performed by both developers and testers                                                | sanity testing is performed by tester alone                                                                                    |
| smoke testing, build may be either stable or unstable                                                    | sanity testing, build is relatively stable                                                                                     |
| it is done on initial builds                                                                             | it is done on stable builds                                                                                                    |
| it is part of basic/acceptance testing                                                                              | it is part of regression testing                                                                                               |
| usually it is done every time there is a new build release                                               | it is planned when there is no enough time to do in-depth testing                                                              |
| Done by the developers and testers                                                                       | Done by testers                                                                                                                |
| Done when the app is unstable                                                                            | Done when the application is stable                                                                                                                               |

![[smoke vs sanity testing.png]]


# Exploratory Testing
- tester have to explore the application, understand completely and test it.
- understand the application, identify all the possible scenarios, document it then use it for testing.
- done when the application is ready but there is no requirement.
- done by test engineer 
	- this depends on the experience of tester

- drawbacks:
	- tester might understand any feature as bug or any bug as feature since they do not have requirement.
	- time consuming
	- if there is any bug in application, you will never know about it (no requirement document).



# Adhoc Testing
- testing application randomly without any test cases or any business requirement document.
- is an informal testing type with an aim to break the system. 
- tester should have knowledge of application even though he does not have requirements/test cases.
- usually unplanned activity.



# Monkey/Gorilla Testing
- testing application randomly without any test cases or any business requirement document.
- is an informal testing type with an aim to break the system. 
- tester do not have knowledge of application.
- suitable for gaming applications.


# Adhoc vs Monkey vs Exploratory Testing

![[adhoc vs monkey vs exploratory testing.png]]




# Positive and Negative Testing

## --Positive Testing
- testing the application with valid input 
- it checks whether an application behaves as expected with positive inputs. 

## --Negative Testing
- testing the application with invalid input 
- it checks whether an application behaves as expected with negative inputs.

 

# End-to-End Testing
- testing the overall functionalities of the system including the data integration among all the modules.


![[end to end testing.png]]




# Globalization and Localization Testing

## --Globalization Testing
- performed to ensure the system or software application can run in any cultural or local environment. 
- different aspects of the software application are tested to ensure that it supports every language and different attributes.
- it teste the different currency formats, mobile number formats and address formats are supported by the application. 
- for example, Facebook.com supports many of the languages and it can be accessed by people of different countries. Hence it is globalized product.

## --Localization Testing
- performed to check system or software application for a specific geographical and cultural environment. 
- localized product only supports the specific kind of language and is usable only in specific region. 
- it tests the specific current format, mobile number format and address format is working properly or not.
- for example, baidu.com supports only the Chinese language and can be accessed only by people of few countries. Hence it is localized product.







