POST is an HTTP method used to submit data to a server to create or update a resource. When a client (e.g., a web browser) makes a POST request, it sends data to the server in the request body, which the server then uses to create or update a resource.

Unlike GET requests, POST requests can modify the server's state and are not considered safe. They should not be cached by intermediaries because the same POST request can have different effects each time it is sent.

Here is an example of a POST request:

```
POST /submit-form HTTP/1.1
Host: example.com
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
Content-Type: application/x-www-form-urlencoded
Content-Length: 23

username=john&password=doe
```

In this example, the client is making a POST request to submit a form with the username and password fields. The `Content-Type` header specifies that the data being sent is in URL-encoded format, while the `Content-Length` header indicates the size of the request body in bytes.

The server will respond to the POST request by creating or updating the resource and returning an HTTP response code indicating whether the request was successful.