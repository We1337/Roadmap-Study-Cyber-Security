PUT is an HTTP method used to update an existing resource on the server. When a client (e.g., a web browser) makes a PUT request, it sends data to the server in the request body to replace the existing resource.

Unlike GET requests, PUT requests can modify the server's state and are not considered safe. They should not be cached by intermediaries because the same PUT request can have different effects each time it is sent.

Here is an example of a PUT request:

```
PUT /api/users/123 HTTP/1.1
Host: example.com
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
Content-Type: application/json
Content-Length: 37

{"name": "John Doe", "email": "john@example.com"}
```

In this example, the client is making a PUT request to update the user with the ID `123`. The request body contains a JSON object with the new values for the user's `name` and `email` fields. The `Content-Type` header specifies that the data being sent is in JSON format, while the `Content-Length` header indicates the size of the request body in bytes.

The server will respond to the PUT request by replacing the existing resource with the new data and returning an HTTP response code indicating whether the request was successful.