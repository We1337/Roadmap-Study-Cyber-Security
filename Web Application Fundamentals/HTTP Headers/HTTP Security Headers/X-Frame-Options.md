X-Frame-Options is an HTTP security header that controls whether or not a web page can be displayed inside a frame or iframe on another site. This can help prevent clickjacking attacks, in which an attacker embeds a page or component from one site inside another site, without the user's knowledge or consent.

When a browser receives a web page with an X-Frame-Options header, it will check the header and take action based on its value. There are three possible values for the header:

1. `DENY`: This value indicates that the page should never be displayed inside a frame, even on the same site. If a browser receives a page with this header, it will simply refuse to display the page inside a frame.
2. `SAMEORIGIN`: This value indicates that the page should only be displayed inside a frame on the same site. If a browser receives a page with this header, it will allow the page to be displayed inside a frame only if the frame is hosted on the same domain as the page itself.
3.  `ALLOW-FROM uri`: This value indicates that the page should only be displayed inside a frame on a specific site. The `uri` parameter should be set to the specific site that is allowed to display the page inside a frame.  

Here is an example of an X-Frame-Options header:

```
X-Frame-Options: SAMEORIGIN
```

This header indicates that the page should only be displayed inside a frame on the same site.

It's important to note that not all browsers support the X-Frame-Options header, and some older browsers may not recognize it at all. Nevertheless, it can be a useful tool in a defense-in-depth strategy for web application security.