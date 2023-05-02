HTTP security headers are HTTP response headers that are used to improve the security of web applications by mitigating various attacks such as cross-site scripting (XSS), clickjacking, cross-site request forgery (CSRF), and others.

Here are some commonly used HTTP security headers:

1. Content-Security-Policy (CSP) - Used to prevent XSS and other code injection attacks by specifying which sources of content are allowed to be loaded by the web application.
2. X-Frame-Options - Used to prevent clickjacking attacks by specifying whether or not a web page can be displayed within an iframe.
3. X-XSS-Protection - Used to prevent XSS attacks by enabling the built-in XSS filter in some web browsers.
4. X-Content-Type-Options - Used to prevent MIME type sniffing attacks by specifying that the web server should only serve files with the MIME type specified in the Content-Type header.
5. Strict-Transport-Security (HSTS) - Used to force web browsers to use HTTPS for all communication with the server, preventing man-in-the-middle attacks and session hijacking.
6. Referrer-Policy - Used to control the information sent in the Referer header when a user clicks on a link to another site. 
7. Feature-Policy - Used to specify which browser features are allowed to be used on a web page.

By using these headers, web application developers can improve the security of their applications and protect against a variety of attacks.