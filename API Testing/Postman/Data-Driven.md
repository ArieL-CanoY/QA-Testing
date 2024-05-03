
### Get all data from CSV or JSON
```python
the name of the variable should be the name when it is refer.

in the csv:
id       name
1        mark
2        vince

in the json:
[
	 {
		"id": 1,
		"name": "mark"
	 },
	 {
		"id": 2,
		"name": "vince"
	 }
]

in the postman, it should be:
body section of request:
{
   "customerId": {{id}},
   "customerName": "{{name}}"
}



```


# Run the collection of request
```python
1. click the kebabr (...) of the collection
2. click run collection
3. select the csv or json file
4. check the number of data, if the last data is null or empty string, subtract 1 to iteration number
5. Run
```




























