pre-request script - execute before the request is send.
tests - execute after the request is sent.

check the request method used 
```javascript
if (pm.request.method === "GET")
```


check the response status
```javascript
if (pm.response.to.have.status(200))
```


different debug
```javascript
console.log()
console.info()
console.warn()
console.error()
```


setting a variable
```javascript
//levels - environment, globals, localVariables, variables
let varName = pm.<levels>.set('varname', 'value')
console.log(varName)
```

getting a variable
```javascript
//levels - environment, globals, localVariables, variables
let varName = pm.<levels>.set('varname')
console.log(varName)
```

















