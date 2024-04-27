
# What
```python
- contains specific data or value
```

# Why
```python
- to avoid duplication
- easy to change reference value to multiple location
- use for specific environment or context
```

# Where
```python
- you can referer the variable to request url, body
```

# Note
```python
- you can overwrite the value of variable 
- REQUEST overwrite ENVIRONMENT overwrite COLLECTION overwite GLOBAL
- REQUEST >> ENVIRONMENT >> COLLECTION >> GLOBAL

```


# Scope
```python
# listing all accessible location

Global:
	anywhere in a workspace
	collection inside a workspace
	request inside a collection

Collection:
	collection - same as above
	request - same as above

Environment:
	anywhere in a workspace: collection, request
	need to switch to different environment
	useful for frequently changing values of variables

Local:
	inside a request
	should be inside the pre-request script
	
Data:
	external files like cvs or text
	

```


# Set variable through script
check the "Test Script" file [[Test Script]] on line 36





















