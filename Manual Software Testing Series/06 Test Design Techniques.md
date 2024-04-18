- Test/Test Case/Test Data Design Techniques is  used to prepare data for testing.
- helps to design better cases.
- reduce the number of test cases to be executed.

In testing, there are so many data/input to test, we can minimize the data and improve the coverage. 

goal:
1. reduce data - input for testing
2. more coverage - cover the scenario based on data

5 types of techniques:
- Equivalence Class Partition (ECP)
- Boundary Value Analysis (BVA)
- Decision Table based testing
- State Transition
- Error Guessing

# Equivalence Class Partition (ECP)
- partition data into various classes and we can select data according to class then test. It reduce the number of test-cases and saves time for testing. 

example:
	enter number between 1-500

normal test data - 1,2,3,4,5,6...500

divide values into equivalence classes:
-100 - 0 > 50 (invalid)
1 - 100 > 30 (valid)
101 - 200 > 160 (valid)
201 - 300 > 250 (valid)
301 - 400 > 320 (valid)
401 - 500 > 450 (valid)
501 - 600 > 550 (invalid)

test data using ECP:
-50
30
160
250
320
450
550

another example:
	name: [     ] \*allow only alphabet
	
test data using ECP:
	XYZ > valid
	xyz > valid 
	@#$% > invalid	
	Xy z > invalid
	1234 > invalid


# Boundary Value Analysis (BVA)
- used to check boundaries of the input.

example:
enter number from 18-35

min: 18 (should pass)
min-1: 17 (should fail)
min+1: 19 (should pass)

max: 35 (should pass)
max-1: 34 (should pass)
max+1: 36 (should fail)

ECP and BVA are used in Input Domain Testing
- The value will be verified in the textbox/input field 


# Decision Table
- also called as Cause-Effect Table.
- used if we have more conditions and corresponding actions.
- deals with combinations of inputs.
- to identify the test cases, we consider conditions and actions. 
- if we have more number of conditions/actions,

![[decision table.png]]


# State Transition 
- changes in input conditions change the state of the application.
- this testing technique allows the tester to test the behavior of an AUT.
- performed by entering various input conditions in a sequence.
- the testing team provides positive as well as negative input test values for evaluating the system behavior.

![[transition state.png]]



# Error Guessing
- one of the testing techniques used to find bugs in a software application based on tester's experience.
- do not follow any specific rules.
- it depends on the Tester Analytical skills and experience.
- Some examples are:
	- submitting a form without values.
	- entering invalid values such as alphabets in the numeric field.



























