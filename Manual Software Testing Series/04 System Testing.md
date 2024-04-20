note: do not assume the functionality, refer to the documentation

- black box testing technique
- testing the software/product depending on customer's requirements


Examples:
- GUI Testing
- Usability Testing
- Functional Testing
- Non-Functional Testing


## Graphical User Interface (GUI) Testing
-  process of testing the user interface of an application
- GUI includes all the elements such as menus, checkbox, buttons, colors, fonts, sizes, icons, content, and images. 
- conducted based on the document of wireframe

![[gui testing checklist.png]]




## Usability Testing
- During the testing, it validates application provided context sensitive help or not to the user
- Checks how easily the end users are able to understand and operate the application



## Functional Testing
- functionality is the behavior of the application
- requirements - it should have this feature, those features


Examples:
- Object Property Testing
	-  check the properties of objects present on the application
	- everything is an object - text, logo, image, dropdown, etc.
	- button if clickable, input if enable, radio buttons if group, etc.

- Database Testing/Backend Testing
	- can be black box or white box testing
	- if beginner (black-box testing):
		- DML Operation (Data Manipulation Language) - Insert, Update, Delete, Select
	- if experienced (white-box testing), should know in-depth of SQL:
		- table level validations (column type, column length, num of columns)
		- relation between the tables (normalization)
		- procedures
		- triggers
		- indexes
		- views
		- etc.

- Error Handling 
	- focus on error message
	- show error to know what happen to the system
	- verify the error messages while performing incorrect actions
	- error messages should be user readable and understandable/simple language

- Calculations/Manipulations Testing
	- financial like banking
	- verify the calculations of the app


- Links Existence and Links Execution
	- Links Existence - where exactly the links are placed
	- Links Execution - links are navigating to proper page or not

	- Types of links:
		- Internal - hyperlinks that direct users to another page of the same website or domain
		- External - hyperlinks that direct users to another website or domain
		- Broken - do not have any hyperlinks or does not direct to another page or website


- Cookies and Sessions
	 - only done in web app
	 - Cookies - temporary files created by browser while browsing the pages through internet
	 - Session - time slots created by the server. Session will expired if idle for sometime




## Non-Functional Testing
- once the application functionality is stable then we do Non-Functional testing
- focus on performance, load it can take, and security, etc.
- expectation for the app - should get the page faster, should be secure, etc.


Examples:
- Performance Testing
	- speed of the app
	- how well the server is responding to request of the clients
	- most performed on web app
	- Examples:
		- Load Testing - gradually increasing the load/data of the application and test the speed
		- Stress Testing - suddenly increasing the load/data of the application and test the speed
		- Volume Testing - check how much data is able to handle by the application
- Security Testing
	- Authentication - verify users are valid or not
	- Authorization/Access Control - verify the permissions of the valid user to do some actions
- Recovery Testing
	- test if something lost, it can immediate recover
	- check the system from abnormal to normal - recovery mechanism
- Compatibility Testing
	- Forward - verify if the device is compatible after the updating to new version of the software
	- Backward - verify if the device is compatible after the downgrading to old version of the software
	- Hardware - verify if the software is compatible to install to different hardware
- Configuration Testing
- Installation Testing
	- check screens are clear to understand
	- screens navigation
	- simple or not to install
	- uninstallation process if all related files are deleted
- Sanitation/Garbage Testing
	- if any application provides extra features/functionality then we consider them as bug



# Functional vs Non-Functional Testing

<table style="width: 100%;">
	<tr>
		<th style="border: 1px solid white; width: 50%; text-align: center; font-size: 30px">Functional Testing</th>
		<th style="border: 1px solid white; width: 50%; text-align: center; font-size: 30px">Non-Functional Testing</th>
	</tr>
	<tr>
		<td style="border: 1px solid white; text-align: center;">Describes what software does</td>
		<td style="border: 1px solid white; text-align: center;">Describes how software works</td>
	</tr>
	<tr>
		<td style="border: 1px solid white; text-align: center;">Validates functionality of Software</td>
		<td style="border: 1px solid white; text-align: center;">Verify the performance, security, reliability of the software</td>
	</tr>
	<tr>
		<td style="border: 1px solid white; text-align: center;">Concentrates on user requirement</td>
		<td style="border: 1px solid white; text-align: center;">Concentrates on user expectation</td>
	</tr>
	<tr>
		<td style="border: 1px solid white; text-align: center;">Takes place before Non-Functional testing</td>
		<td style="border: 1px solid white; text-align: center;">Performed after finishing Functional testing</td>
	</tr>
</table>



































