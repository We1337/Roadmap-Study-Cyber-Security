Accessing unresolved DNS entries via the Host header is a technique that involves sending HTTP requests with a specific Host header to a web server. This technique is sometimes referred to as "Host Header Injection" or "Virtual Host Poisoning."

The idea behind this technique is to manipulate the Host header in the HTTP request and set it to a domain or hostname that is not resolved in the DNS. By doing so, you can potentially bypass any DNS-based filtering or routing mechanisms and reach the target server.

Here's a basic overview of how it works:

1. Craft an HTTP request: Create an HTTP request (usually using tools or scripting) where you set the Host header to the domain or hostname you want to access.
2. Send the request: Send the HTTP request to the target server and observe the response. 
3. Analyze the response: The target server may respond in different ways depending on its configuration. It could respond with a default virtual host, an error page, or redirect you to a different location.

It's important to note that accessing unresolved DNS entries via the Host header can have unintended consequences, such as triggering unexpected behavior on the target server or potentially violating the server's usage policies. Always ensure you have proper authorization from the server owner or follow responsible disclosure practices if you discover any vulnerabilities.

Additionally, it's worth mentioning that some web servers and hosting providers have measures in place to prevent or mitigate Host header injection attacks. This could include configuration settings, server-side filtering, or other security measures.

Please keep in mind that this information is provided for educational purposes only. It's essential to always comply with the law and obtain proper authorization before conducting any testing or research activities.