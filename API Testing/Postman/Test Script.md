pre-request script - execute before the request is send.
tests - execute after the request is sent.

```python
var - can reassign the value of a variable once it is declared.

const - cannot reassign the value of a variable once it is declared, it will throw an error.
```

### eql vs equal
```python
eql - compare if an object is the same value with another object.

equal  - compare if an object is the same reference with another object - memory reference.

note: use eql if you want to compare the exact the same value.




```



### different debug options
```javascript
console.log()
console.info()
console.warn()
console.error()
```


### setting a variable
```javascript
//levels - environment, globals, localVariables, variables
let varName = pm.<levels>.set('varname', 'value')
console.log(varName)
```

###  getting a variable
```javascript
//levels - environment, globals, localVariables, variables
let varName = pm.<levels>.set('varname')
console.log(varName)
```

### arrow function 
```python
pm.test("Testing title", ()=> {
	//assertion here
});
```

# Assertions


### check the request method used 
```javascript
if (pm.request.method === "GET")
```


### check the response status
```javascript
if (pm.response.to.have.status(200))
```


defines an arrow function test case with description of "Status code is 200" and expecting to have response status code of 200
```python
pm.test("Status code is 200", ()=>{
    pm.response.to.have.status(200)
})
```


test the response status code to be one in the array
```python
pm.test("Status code is 200", ()=>{
    pm.expect(pm.response.code).to.be.oneOf([200,201,202])
})
```



# Validate Headers

check if specific header is present in the response
```python
 pm.response.to.have.header("Content-Type");
```

check the value of specific header
```python
pm.expect(pm.response.headers.get("Content-Type")).to.equal("application/json")
```



# Validate Cookies

check if the specific cookie is present in the response
```python
pm.test("Response has a cookie set named session", ()=> {
    pm.expect(pm.cookies.has("session")).to.be.true;
});
```

check the value of specific cookie 
```python
pm.test("response cookie named oai-did has a value of 57fe87cb-886a-4d0e-bca0-de1369a2f742", ()=> {
    pm.expect(pm.cookies.get("oai-did")).to.equals("57fe87cb-886a-4d0e-bca0-de1369a2f742");
});
```



# Validate Response Time

#### Below or less than
```python
# note that the value is in milliseconds
pm.test("Response time is less than 1000ms", ()=> {
    pm.expect(pm.response.responseTime).to.below(1000);
	#or
    pm.expect(pm.response.responseTime).to.lessThan(1000);
});
```

### Above or greater than
```python
# note that the value is in milliseconds
pm.test("Response time is less than 1000ms", ()=> {
    pm.expect(pm.response.responseTime).to.above(1000);
	#or
    pm.expect(pm.response.responseTime).to.greaterThan(1000);
});
```


### Within or between
```python
pm.test("Response time is within 200ms to 300ms", ()=> {
    pm.expect(pm.response.responseTime).to.be.within(200, 300);
});
```




# Validate response body

# JSON

### Validating JSON data types 

```python
# declare a variable that will capture the json response 
const jsonData = pm.response.json();

pm.test("JSON data type testing", ()=> {
    pm.expect(jsonData).to.be.an("object");
    pm.expect(jsonData.id).to.be.an("string");
    pm.expect(jsonData.phone).to.be.an("string");
    pm.expect(jsonData.courses).to.be.an("array");
});

```



### Validating JSON data values and include
```python
var jsonData = pm.response.json();

pm.test("JSON data values testing", ()=> {
    pm.expect(jsonData.id).to.eql("1");
    pm.expect(jsonData.phone).to.eql("09847586958");
    pm.expect(jsonData.courses).to.eql(["Java","Selenium"]);
    pm.expect(jsonData.courses[0]).to.eql("Java")

	//include or have array of
	pm.expect(jsonData.courses).to.include("Java");
	pm.expect(jsonData.courses).to.have.members(["Selenium","Java"]);
});
```



### Validating JSON schema
```python
//tv4 is like pm, built in class, but jsonData and schema should specify their value

var jsonData = pm.response.json();
var schema = {
  "$schema": "http://json-schema.org/draft-04/schema#",
  "description": "",
  "type": "object",
  "properties": {
    "id": {
      "type": "string",
      "minLength": 1
    },
    "name": {
      "type": "string",
      "minLength": 1
    },
    "location": {
      "type": "string",
      "minLength": 1
    },
    "phone": {
      "type": "string",
      "minLength": 1
    },
    "courses": {
      "type": "array",
      "items": {
        "required": [],
        "properties": {}
      }
    }
  },
  "required": [
    "id",
    "name",
    "location",
    "phone",
    "courses"
  ]
}

//validation
pm.test("JSON schema", ()=> {
    pm.expect(tv4.validate(jsonData, schema));
});
```


























