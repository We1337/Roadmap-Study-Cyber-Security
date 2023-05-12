DELETE is an HTTP method used to delete a resource on the server. When a client (e.g., a web browser) makes a DELETE request, it asks the server to remove the resource specified in the request URI.

Unlike GET requests, DELETE requests can modify the server's state and are not considered safe. They should not be cached by intermediaries because the same DELETE request can have different effects each time it is sent.

Here is an example of a DELETE request:

```
DELETE /api/users/123 HTTP/1.1
Host: example.com
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
```

In this example, the client is making a DELETE request to remove the user with the ID `123`. The request URI specifies the resource to be deleted, while the headers provide additional information about the request.

The server will respond to the DELETE request by removing the specified resource and returning an HTTP response code indicating whether the request was successful.