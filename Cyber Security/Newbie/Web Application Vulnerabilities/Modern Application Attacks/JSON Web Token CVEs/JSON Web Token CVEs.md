JSON Web Tokens (JWTs) have been subject to various Common Vulnerabilities and Exposures (CVEs) over time. Here are some notable CVEs related to JSON Web Tokens:

1.  CVE-2015-2951: This vulnerability affected the JavaScript Object Signing and Encryption (JOSE) library, which is commonly used for JWT processing. It allowed an attacker to bypass signature verification and modify the contents of a JWT.
2.  CVE-2016-10555: This vulnerability impacted some JWT libraries and allowed an attacker to bypass signature validation by modifying the "alg" header parameter to specify an algorithm that was not supported by the server.
3.  CVE-2018-0114: This vulnerability affected the Nimbus JOSE+JWT library and allowed an attacker to bypass signature verification by exploiting a flaw in the library's handling of certain JWS/JWT header values.
4.  CVE-2019-12326: This vulnerability affected the "jsonwebtoken" library for Node.js and allowed an attacker to bypass signature verification by specifying an algorithm that was not supported by the server.
5.  CVE-2020-10531: This vulnerability impacted the "auth0-js" library and allowed an attacker to modify the "nonce" parameter in the JWT authentication flow, potentially leading to replay attacks.

It's important to note that the CVEs mentioned above are specific to certain libraries or implementations of JWTs and may not directly impact the JWT specification itself. However, they highlight potential security issues that can arise when using JWTs in applications.

To mitigate the risks associated with these vulnerabilities and ensure the secure usage of JWTs, consider the following best practices:

1.  Keep Libraries and Dependencies Up to Date: Regularly update the JWT libraries and related dependencies to the latest secure versions that address any known vulnerabilities.
2.  Validate JWT Signatures: Implement robust signature validation to ensure the integrity and authenticity of the JWT. Verify that the signature algorithm and key used to sign the JWT are trusted and properly validated.
3.  Use Supported and Secure Algorithms: Limit the accepted algorithms for JWT signing and verification to those that are widely supported, well-vetted, and considered secure (e.g., HMAC-SHA256 or RSA-SHA256).
4.  Validate JWT Claims and Data: Perform thorough validation of the JWT claims and data, such as expiration dates, issuer, and audience, to ensure that the JWT is used within its intended scope and lifetime.
5.  Implement Proper Access Controls: Combine JWTs with appropriate access control mechanisms to enforce authorization rules and restrict access to sensitive resources or actions.
6.  Secure Storage and Transmission: Safeguard JWTs during storage and transmission by using secure channels (e.g., HTTPS) and applying appropriate encryption and protection measures to prevent unauthorized access or tampering.
7.  Implement JWT Expiration and Revocation: Set reasonable expiration times for JWTs and consider implementing mechanisms for token revocation, such as token blacklisting or using short-lived JWTs.
8.  Security Testing: Conduct security assessments, including penetration testing and code reviews, to identify any implementation flaws or vulnerabilities specific to JWT usage in your application.

By following these best practices and staying updated on security advisories related to JWT libraries, you can mitigate the risks associated with known CVEs and ensure the secure implementation and usage of JSON Web Tokens.