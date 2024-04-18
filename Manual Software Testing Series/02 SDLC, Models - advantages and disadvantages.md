
#### SDLC
Software Development Life Cycle
	- a process used by software industry to design, develop and test software

3 pillars of a company:
	P - People - developer, staff, manage
	P - Process - protocols and rules to obey to achieve goal. To design, develop, test, deliver
	P - Product - what a company delivered to a customer


#### SDLC Process
Requirements Analysis>>Design>>Development>>Testing>>Maintenance

- Requirements Analysis
	- gather the information or collect the requirements from the customers

- Design
	- The designers will design the software. Making a blueprint. How it should look like - navigations, buttons, functions.

- Development
	- Software developers will develop programs with different kinds of programming languages.

- Testing
	- After development is completed, before delivering the software to the customer, is has to be tested. Conduct different kind of testing like functional and non-functional, security, etc.

- Maintenance
	- After delivered the software, maintenance should start. This is the deployment phase where customer used the software made by the developer. 



# ------------------ SDLC Models ------------------




##  ---------- Waterfall Model ----------

![[waterfall model.png]]

   - very old model - does not used nowadays
   - waterfall is like flowing water, there is no going back after the development so that make sure that every phases of development is quality
   - documentation plays an important role on this model

#### Waterfall Model Process:
	   - Requirement Analysis - gather all the requirements from the customer and after that, they prepare SRSD (Software Requirement Specification Document)
	   - System Design - based on the document, different teams will design the software that is divide in two level which is low and high level view of the software 
	   - Implementation - they will integrate it once the system design is finished
	   - Testing - test the quality of the software 
	   - Deployment - deploy the software on the customer environment, install the software, documentation of the software, user manual.
	   - Maintenance - customer will start using the software

#### Advantages of Waterfall Model
	1. Quality of the software will be good.
		- Every phases has a detailed document
	2. Chances of finding bugs will be less.
		- Since requirement changes are not allowed
	3. Initial investment is less.
		- Since the tester will hire later on the stage  
	4. Preferred for small projects where requirements are freeze. 
	
#### Disadvantages of Waterfall Model
	1. Requirement changes are not allowed.
		- because it is freeze model, cannot go back from previous phases
	2. If there is defect in Requirements that will be continuued in later phases.
		- if the first phase is wrong, then the later phases will affect
	3. Total investment is more.
		- because time taking for rework on defect is time consuming which leads to higher investments.
	4. Testing will start only after coding.
		-  after the completion of the implement of the design








## ---------- Spiral model ----------

![[spiral model.png]]
   
   - old model - does not used nowadays
   - overcome the drawbacks of Waterfall model such as changes, flow control, repetitions
   - the difference is this model accommodate new and changes in the requirements
   - an iterative model - repeatable process
   - used whenever there are dependency on the modules 
   - in every cycle, new software/version/model will be released to the customer
   - software will be released in multiple versions, so it is called version control model

   
#### Spiral Model Process:
	   - Planning - Requirement Analysis
	   - Risk Analysis - Prototype - how much risk are involved, how many developers and testers are required in detailed
	   - Engineering and Execution - Design and Development
	   - Evaluation - Customer Evaluation - testing and maintenance

1st Cycle
![[spiral model 1st cycle.png]]
 
2nd Cycle
''

#### Advantages of Spiral Model
	1. Testing is done in every cycle, before going to the next cycle
		- Every phases will conduct testing because it is iterative and can have many cycle 
	2. Customer will get to use the software for every module
		- Customer does not need to wait to complete the software and immediately use or test it after a cycle
	3. Requirement changes are allowed after every cycle before going to the next cycle.
		- changes are allowed after the completion or before to start o a/another cycle and not in the middle of the cycle or phases  
	
#### Disadvantages of Spiral Model
	1. Requirement changes are not allowed in between the cycle.
		- only after the completion of the cycle or before a/another cycle will start
	2. Every cycle of spiral model looks like waterfall model.
		- because it has one (1) phase of testing every cycle
	3. There is no testing in requirement and design phase
		- additionally for number two (2) which it will not test the software properly


#### Prototype overview
Process:
	Initial requirements from the customer >> Prototype >> Customer >> design, coding, testing




## ---------- V/VV model ----------

![[V model.png]]
   
   - VV stands for verification and validation 
   - every part of cycle or the phases, it will conduct testing
   -  

#### V Model Process:

<html>
	<style>
		#table
		{
			border: 1px solid white;
		}
	</style>
	
	<body>
		<table>
		<tr>
			<td style="border: 1px solid white; width: 50%">VERIFICATION</td>
			<td style="border: 1px solid white; width: 50%">VALIDATION</td>
		</tr>
		<tr>
			<td style="border: 1px solid white;">BRS/CRS/URS - Business Requirement Specification, Customer '', User ''. This cannot understand by the developer or testers and only business people can understand so SRS will be prepare. This will prepare by business unit/people</td>
			<td style="border: 1px solid white;">Black Box Testing will conduct for this specification specifically User Acceptance Testing (UAT)</td>
		</tr>
		<tr>
			<td style="border: 1px solid white;">SRS (Software Requirements Specification) - document for the developers and testers of the application and it will present in a presentation such as Venn diagram, flow chart. This will prepare by project manager</td>
			<td style="border: 1px solid white;">Black Box Testing will conduct for this specification specifically System Testing</td>
		</tr>
		<tr>
			<td style="border: 1px solid white;">1. High Level Design (HLD) document - including the design of different modules
			2. Low Level Design (LLD) document - including the design of different sub modules which is more detailed than modules. This two (2) documents will prepare by designers.  </td>
			<td style="border: 1px solid white;">White Box Testing will conduct for different modules specifically Integration Testing - testing the integrate of a module to different module if they are working properly together. </td>
		</tr>
		<tr>
			<td style="border: 1px solid white;">Coding - which the development will  start. This will prepares by developers.</td>
			<td style="border: 1px solid white;">White Box Testing will conduct for this functionality specifically Unit Testing - testing the logic of the code</td>
		</tr>
		
		</table>
	</body>
</html>


Static testing - testing the project related to document
	By using 3 different techniques, it can verify all the documents by using:
		1. Review
		2. Walkthrough
		3. Inspection

Dynamic testing - testing the actual software
	Some of techniques are:
		1. Unit testing
		2. Integration testing
		3. System testing
		4. User Acceptance testing

After coding it will conduct:
1. Unit Testing - test one module or part of the system if it is align with the design especially the logic of the system. This will be test by the developer.
2. Integration testing - test the integration of two or more modules if they will should together as expected. This will be test by the developer.
3.  System Testing - conducted by the testing team which does not require programming knowledge because it is black box testing which test only as the perspective of a user and a technical tester if the functionalities is working properly based on the customer requirements in the document.
4. User Acceptance Testing (UAT) - this test will conduct by the customers along with the testers


### Verification vs Validation

####     Verification
		- checks whether we are building the right product
		- Focus on documentation
		- Verification typically involves:
		- Reviews, Walkthroughs,  Inspections
	
####     Validation
		- checks whether we are build the product right
		- Takes place after verifications are completed
		- Focus on Software
		- Validation typically invovles actual testing
		- Unit testing, integration, system, and UATesting
	

#### Advantages of V Model
	1. Testing is involved in each and every phase
	
#### Disadvantages of V Model
	1. Documentation is more
		- this will need to validate the system based on the documents 
	2. Initial investment is more
		- because it has to verify documents and validate the output thoroughly
