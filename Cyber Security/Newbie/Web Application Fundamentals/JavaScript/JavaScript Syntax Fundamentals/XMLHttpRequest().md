`XMLHttpRequest()` is a built-in JavaScript object that allows you to make HTTP requests to a server and retrieve data in various formats, such as JSON, XML, or HTML. It is commonly used in web development to create dynamic and interactive web applications that communicate with web servers.

Here's an example of how to use `XMLHttpRequest()` to make a GET request to a server:

```javascript
// create a new XMLHttpRequest object
var xhr = new XMLHttpRequest();

// specify the URL of the resource to be retrieved
xhr.open('GET', 'https://example.com/api/data');

// set the response type
xhr.responseType = 'json';

// define a callback function to handle the response
xhr.onload = function() {
  // check the response status
  if (xhr.status === 200) {
    // handle the response data
    console.log(xhr.response);
  } else {
    // handle the error
    console.log('Error: ' + xhr.status);
  }
};

// send the request
xhr.send();
```

In this example, we first create a new `XMLHttpRequest()` object using the `new` keyword. We then call the `open()` method on the object to specify the URL of the resource to be retrieved and the HTTP method to be used (`GET` in this case). We also set the `responseType` property to `'json'`, indicating that we expect the response data to be in JSON format.

Next, we define a callback function to handle the response. This function is assigned to the `onload` property of the `XMLHttpRequest()` object and is executed when the response is received. In this example, we check the status of the response using the `status` property, and if it is `200` (indicating a successful response), we log the response data to the console. If the status is not `200`, we log an error message instead.

Finally, we call the `send()` method on the `XMLHttpRequest()` object to send the request to the server. The server responds with the requested data, which is then processed by the callback function.