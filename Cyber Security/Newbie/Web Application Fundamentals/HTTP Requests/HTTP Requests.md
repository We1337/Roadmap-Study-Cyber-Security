HTTP requests are the messages sent by a client (e.g., a web browser) to a server, in order to initiate an action or retrieve a resource. HTTP requests are composed of a request line, request headers, and an optional request body.

The request line consists of the HTTP method, the URL of the resource being requested, and the version of the HTTP protocol being used. Here is an example of a request line:

```
GET /index.html HTTP/1.1
```

This request line indicates that the client is making a GET request for the `index.html` file, using the HTTP/1.1 protocol.

After the request line, the client may include request headers, which provide additional information about the request or the client making the request. Request headers are key-value pairs separated by a colon, and multiple headers can be included in a single request. Here is an example of a request header:

```
Host: example.com
```

This header indicates that the client is requesting a resource from the `example.com` domain.

Finally, if the request requires a body, such as in the case of a POST request, the body is included after the headers, separated by a blank line. The body can contain any data that needs to be sent to the server as part of the request.

HTTP requests can be made using various methods, including GET, POST, PUT, DELETE, and others. The most commonly used methods are GET and POST. A GET request is used to retrieve a resource, while a POST request is used to submit data to the server for processing. The method used for a request is specified in the request line.