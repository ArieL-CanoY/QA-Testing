# Definition
```python
- a set of rules and protocols that allows different programs to communicate or share data.
- API allows a program to access data from another program that 
- API is a service commonly for the websites.
- API Medium is HTTP and the format is XML/JSON/Text.

```



# Types of API
```python
1. SOAP (Simple Object Access Protocol) 
	- old technology
	- HTTP methods:
		-- POST only
	- Data communcation format is only XML
	- XML messages or data should have defined structure which is SOAP message that consists the following:
		-- Envelop - root element of the 
		-- Header (Optional) - information about the message, might include authenticatoin.
		-- Body - contains the actual data to be send.




2. REST (Representation State Transfer)
	- new technology
	- HTTP methods:
		-- GET, POST, PUT, PATCH, DELETE, TRACE, HEAD, OPTIONS
	- Data communication format is JSON, Text, and XML
		- Commonly use JSON and Text data format to for exchanging information across different systems.
	

```




# Payloads
```python
- the body in the HTTP request and response message.
```



# Web Terms
```python
https://www.mywebsite.com/article/blog

>> https
	- scheme/protocol

>> www
	- subdomain

>> mywebsite
	- domain

>> com
	- top-level domain (TLD)

>> /article/blog
	- endpoint




```


# WSDL and UDDI
```python
>> WSDL (Web Service Description Language)
	- It is used for describing the functionality of a SOAP based web service.
	- XML based interface to describe the details and how a webservice should used.
	- This is like a documentation on how to an API but only the XML are shown and no description of text.
	- If the service consumer and provider knew each other, they can directly communicate with the WSDL.
	- We can say that it is an end point where the service is running.
	- Defining it would require the following:
		- type
			- message
		- porttype
			- operation
			- input
			- output
		- binding
		- service
			- port


			





>> UDDI (Universal Description, Discovery and Integration)
	- If the service consumer and provider does not know each other, they can search a service to the UDDI which has the directory of all the WSDL which the service served.
	- Web service provider publish their WSDL in UDDI to be found by other customer/client who want to use their services via WSDL.
	- 


```


# WSDL message part

### Input message
```xml
<message name=EmployNameRequest>
	<part name="EmployID" type="xsd:number"/>
</message>
```

### Output message
```xml
<message name=EmployNameResponse>
	<part name="EmployName" type="xsd:string"/>
</message>
```




# JSON
```python
- stands for JavaScript Object Notation
- standard for submitting or reading data from or to the server

```

# HTTP Requests
```python
>> GET
	- retrieve resource from the database
	- response code - 200 OK

>> POST
	- create resource on the database
	- response code - 201 Created

>> PUT
	- update existing resource on database, should specify all the information, if partial, use PATCH request.
	- response code - 


>> PATCH
	- update partial existing resource on database
	- response code - 204 No Content

>> DELETE 
	- delete existing resource from database
	- response code - 204 No Content

```


# API Testing
```python

Validates HTTP:
	response status code
	response body
	size
	time taken
	cookies
	headers
	

```
















