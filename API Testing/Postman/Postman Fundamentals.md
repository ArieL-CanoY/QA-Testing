# Definition
```python
- an API testing tool
- support Desktop and Web version



```


# Workspace
```python
- area where we maintain files and saved.

```

# Collections
```python
- contains files and different types of HTTP request
```



# Pre-request and Test Script
```python
- allows us to execute test before sending request or after getting response.

Pre-request script tab
	- execute script before the request is send.

Test script tab
	- execute script after getting a response.
```

### Features
```python
- you can set pre-request and test script on the collection, folder, and request
```

### Execution
```python
- if you have set pre-request and test script to collection, folder, and request, the execution flows is:

collection (pre-request) >> folder (pre-request) >> request (pre-request) >> request >> response >> collection (test) >> folder (test) >> request (test)
```

Here is the visual presentation:
![[postman script execution flow.png]]



















