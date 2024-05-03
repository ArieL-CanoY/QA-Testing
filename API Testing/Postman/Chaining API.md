

```python
in the first request, write a test script that will get the response to json then set specific value of that json to specific levels (global, environment, collection). The remaining request can used that variable to access the response json data from the first request


explanation:
1st request >> response >> to json data >> set specific data to a level >> 2,3,4,5,etc. request should access the (level) variable in their pre-request script.
```



# Random characters generator
```javascript

//useful for dynamic data
function GenerateNumber(length)
{
    var result = "";
    const characters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
    const character_length = characters.length;
    const randomVal = Math.random() * character_length;

    for (var index = 0; index < length; index++)
        result += characters.charAt(Math.floor(Math.random() * character_length));
   
    return result
}

const randomVal = GenerateNumber(10);
console.log(randomVal)


  
// set it to the globals level with variable called "name"
pm.globals.set("name", randomVal);


In the body section of the request, change the value of json with double quote like this:
{
	"name": "{{name}}"
}

```

### Shortcut random
```javascript
// Math.random() produce 0.xxxxx to 1.xxxxxxx. it will convert to base 36 (toString(36)) which has 0-9 and a-z. and the substring will return from (1 or 0).(a7s8f7a56ds - arbitrary) to a7s8f7a56ds only

const myvar = Math.random().toString(36).substring(2);
console.log(myvar)


```





