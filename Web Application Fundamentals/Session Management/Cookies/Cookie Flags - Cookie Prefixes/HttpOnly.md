HttpOnly is a flag that can be added to HTTP response headers to indicate that a cookie should not be accessible to client-side scripts, such as JavaScript. When the HttpOnly flag is set, the cookie can only be accessed by the server and is not visible to JavaScript or other client-side scripts. This helps to prevent cross-site scripting (XSS) attacks, where an attacker injects malicious scripts into a website to steal user data, including cookies.

By default, cookies are accessible to both the server and client-side scripts, which means that any script running on the same domain as the cookie can read its contents. This can be a security risk if the cookie contains sensitive information, such as user credentials or session identifiers.

When the HttpOnly flag is set, the cookie is protected from client-side scripts, which significantly reduces the risk of XSS attacks. However, it is important to note that the HttpOnly flag does not provide complete protection against all forms of XSS attacks, particularly those that exploit vulnerabilities in the web application itself.

The HttpOnly flag can be added to a cookie by setting the HttpOnly attribute in the Set-Cookie header of an HTTP response. For example, the following header sets a cookie with the HttpOnly flag:

```
Set-Cookie: myCookie=myValue; HttpOnly
```

It is recommended to use the HttpOnly flag for cookies that contain sensitive information, such as session identifiers, to prevent them from being accessed by client-side scripts. However, it is important to note that the HttpOnly flag should not be used as a replacement for other security measures, such as input validation, output encoding, and secure communication channels, which are also important for preventing XSS attacks.