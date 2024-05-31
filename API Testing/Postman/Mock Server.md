
# Definition
@Postman
```python
Postman enables you to create _mock servers_ to assist with API development and testing. A mock server simulates the behavior of a real API server by accepting requests and returning responses. By adding a mock server to your [collection](https://learning.postman.com/docs/sending-requests/create-requests/intro-to-collections/) and adding [examples](https://learning.postman.com/docs/sending-requests/response-data/examples/) to your requests, you can simulate the behavior of a real API.

When you send a request to a mock server, Postman matches the request to a saved example in your collection. Postman then responds with the data you added to the example. To view existing mock servers in your workspace, select Mock Servers in the sidebar.
```



# Implementation
!! NOTE !! - assuming there is no authentication or authorization involve because this is just for testing only


### GET Request
```python
> create a collection that will serve a mock collection for mock server

> add request to that collection like GET

> click the 3 horizontal dots on the right side of the collection to view more actions then select "Mock Collection"

> add mock server name

# check the checkbox saying "Save the mock URL ..." so you can refer {{$url}} as the URL of the mock server later when requesting.

> copy the link provided

> go to the mock collection > variables > enter "url" in "Variable" field and paste the URL in the "Initial value" and "Current value" and save.

> click the 3 horizontal dots to the "Request" inside the collection and click "Add example"

> in the url section, refer the variable name by typing "{{url}}" then specify endpoint like "{{url}}/users"

> on the bottom, specify the response body that API should provide.

```


































