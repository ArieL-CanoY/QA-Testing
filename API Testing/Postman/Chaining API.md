

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
```







