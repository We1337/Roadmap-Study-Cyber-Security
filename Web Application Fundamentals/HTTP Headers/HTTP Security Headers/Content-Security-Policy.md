Content-Security-Policy (CSP) is an HTTP security header that allows website owners to define and restrict the sources of content that a web browser can load on a web page. By specifying a set of rules for allowable content sources, CSP can prevent cross-site scripting (XSS) attacks, clickjacking, and other types of attacks that rely on the injection of malicious content into a web page.

CSP works by allowing website owners to specify a whitelist of content sources, and then blocking all other sources of content that are not explicitly allowed. This can include external scripts, images, fonts, and other resources. CSP can also be used to prevent the use of certain types of risky features, such as inline script and style tags, which are often used in XSS attacks.

Here is an example of a CSP header:

```
Content-Security-Policy: default-src 'self' https://trusted.com; img-src 'self' https://*.cdn.com;
```

This CSP header allows resources to be loaded from the website itself (`'self'`) and from the domain `https://trusted.com`. It also allows images to be loaded from the website itself (`'self'`) and from any subdomain of `https://cdn.com` using HTTPS. All other resources and sources of content will be blocked.

CSP is a powerful security tool that can help protect websites and their users from a variety of attacks, but it must be used carefully and with knowledge of how it works. Improperly configured CSP headers can break website functionality and prevent legitimate content from being loaded.