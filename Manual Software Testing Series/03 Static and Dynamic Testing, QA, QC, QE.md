D:\Missing File\Learn QA Testing\Manual Testing Full Course - SDET QA Automation Techie


## Static Testing Techniques
- focused on the documentation part
- before the development of the application start

Examples:
	- Review
	- Walkthrough
	- Inspection



#### Review
- conducts on documents to ensure correctness and completeness
- anything can be done by anyone - developer, tester, manager
- can be done anytime

Examples:
	- Requirement Reviews - after gathering all the requirements from the customer, to understand the requirement better, if each requirement mention or not, correct or not 
	- Design Reviews - low and high level documents, diagrams and pictures
	- Code Reviews - the code of developers will be test also by developers using unit testing, review if the code is done correctly like its syntax and logical, whether following proper coding standard
	- Test Plan Reviews - ensure that the test plan is clear, realistic, and covers all the relevant aspects of the software
	- Test cases Reviews etc.


#### Walkthrough
- informal, meaning don't have specific plan, meeting or time
- Author read the document or code and discuss with peers - Author mean the creator of the document
- it's not pre-planned and can be done whenever required
- does not have minute of the meet
- two or more people peers - peers are people working with you or your team or people that are involve in the work


#### Inspection
- most formal review type
- at least 3-8 people will sit in the meeting 1-reader 2-writer 3-moderator plus concerned
	- Reader - author of the document
	- Writer - note down all the question and clarification what have discussed in the meeting
	- Moderator - mediator between other and the rest of the team. Organizer of the meeting
- will have a proper schedule which will be intimated via email to the concerned developer/tester. Writer will note down the minutes of meeting, sometimes moderator does it



## Dynamic Testing Techniques
- by the time dynamic testing, the software is ready
- coding part is done
- focused on the software which are developed

Examples:
	- Unit Testing - the developer will test the code
	- Integration Testing - when integrate multiple modules/components, it will check the data flow of each component if they properly communicate with each other
	- System Testing - can be security testing, UI testing done by the testers
	- User Acceptance Testing (UAT) - done by the testers along with the customers. Set the environment where the customers are going to work - install the software and test the software


# QA, QC, QE
- QA - Quality Assurance
- QC - Quality Control
- QE - Quality Engineer


## QA vs QC

#### Quality Assurance 
- is process related 
- all throughout the SDLC process
- focuses on building in quality
- preventing defects
- process oriented

#### Quality Control
- is the actual testing of the software
- only in the testing phase of the SDLC process
- focuses on testing for quality
- is detecting defects
- product oriented



## Quality Engineer
- writing a code to test the quality of the software


## Levels of testing
- Unit Testing - test the unit or a component of a system
- Integration Testing - testing the combination of multiple component if they properly communicate
- System Testing - testing the overall functionality of the application, every requirement
- User Acceptance Testing (UAT) - testers and users will test the software


### Unit Testing
- a unit is a single component or module of a software
- conducts on a single program or single module
- white box testing technique
- conducted by the developers
- Unit testing techniques:
	- basis path testing - every lines of code should executed
	- control structure testing:
		- conditional coverage - developer/s will verify the conditions using positive and negative inputs
		- loops coverage - developer/s will verify the output and number of loop based on its conditions
	- mutation testing - testing a condition by entering different set of inputs if it outputs correctly



### Integration Testing
- performed between 2 or more modules
- focuses on checking data communication between multiple modules
- is white box testing technique
- Types of Integration testing:
	- Incremental Integration Testing - Incrementally adding the modules and testing the data flow between the modules.
		  3 Approaches:
					  - Top Down - Ensure the module added is the child of previous module. Examples is the parent is composing an email and the child is sent emails and the parent can be sent emails and the child is deleted emails.
					  - Bottom Up - Ensure the module added is the parent of the previous module.
					  - Sandwich/Hybrid - combination of top down and bottom up
					  
	- Non-Incremental Integration Testing - integrate the module all at once
		- drawbacks:
			- miss data flow between some of the modules
			- finding any defect cannot understand the root cause of that defect




### System Testing
- testing overall functionality of the application with respective client requirement
- black box testing technique
- conducted by testing team
- conducted after completion of component and integration level testing 
- before conducting system testing we should know the customer requirements.
- focuses on below aspects:
	- User Interface Testing (GUI)
	- Functional Testing
	- Non-Functional Testing
	- Usability Testing



### User Acceptance Testing
- after completion of system testing, UAT team UAT in two levels:
	- Alpha testing
	- Beta testing



