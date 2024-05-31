

# Basic Auth
```python
>> Basic Auth
	- sending username and password with each request. The credentials are in plaintext or encoded using Base64 that is easily reversible.

url: https://postman-echo.com/basic-auth
username: postman
password: pasword

header content in the first request that will received a 401 response:
WWW-Authenticate: Basic realm="Users"

format in header:
Authorization: Basic <credentials_here(username:password) - plaintext or base64 encoded>
```


# Digest Auth
```python
>> Digest Auth
	- With Digest auth, the client sends a first request to the API, and the server responds with a few details, including a number that can be used only once (a _nonce_), a realm value, and a `401` unauthorized response. You then send back an encrypted array of data including a username and password combined with the data received from the server in the first request. The server uses the passed data to generate an encrypted string and compares it against what you sent to authenticate your request. @Postman
	- just like Basic Auth but more secured by hashing and encrypting the value of username and password when sending over the network.

url: https://postman-echo.com/digest-auth
username: postman
password: pasword


header content when sending the first request that will got 401 HTTP response status code:
WWW-Authenticate: Digest realm="Users", nonce="gz2Ncqz5AEv4IkgePYzN5VKp8lnl80CZ", qop="auth"


for more details, watch this on YT: https://www.youtube.com/watch?v=MKQQ0BSyZ6s
```


# Bearer Token
```python
>> Bearer Token
	- Bearer tokens enable requests to authenticate using an access key, such as a JSON Web Token (JWT). The token is a text string, included in the request header. In the request "Authorization" tab, select "Bearer Token" from the "Type" dropdown list. In the "Token" field, enter your API key value. For added security, store it in a variable and reference the variable by name. @Postman
	- just like token in Github - ghp_klasdf89a98asas9df0




```
































