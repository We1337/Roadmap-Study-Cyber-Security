POODLE, which stands for "Padding Oracle On Downgraded Legacy Encryption," is a security vulnerability that affects the SSLv3 and earlier versions of the TLS (Transport Layer Security) protocols. It was discovered in 2014 and is categorized as a cryptographic attack.

The vulnerability takes advantage of the way SSLv3 handles padding during encryption. Padding is added to plaintext data to ensure that the data being encrypted aligns with the block size of the encryption algorithm. In SSLv3, if the padding is incorrect, the server sends an error message. An attacker can exploit this behavior to gradually decrypt the contents of encrypted messages by forcing the server to repeatedly decrypt and send back small parts of the message.

Here's how the attack works:

1. The attacker intercepts the encrypted traffic between the client and server that is using SSLv3.
2. The attacker downgrades the connection to use SSLv3 if the server and client support it.
3. The attacker injects specially crafted requests into the connection and observes the server's responses.
4. By analyzing the error messages from the server, the attacker gradually learns about the plaintext content of the encrypted messages.

This attack can potentially expose sensitive information, such as cookies, session tokens, and other data that is meant to be confidential.

To mitigate the POODLE attack, it's recommended to disable SSLv3 and use more secure versions of the TLS protocol, such as TLS 1.2 or higher. In fact, due to the discovery of POODLE and other vulnerabilities, SSLv3 has been considered insecure and deprecated by security experts, and its use should be avoided.

As of my last update in September 2021, many web servers and clients have disabled support for SSLv3, and modern browsers no longer use it by default. However, it's important to stay informed about the latest security best practices and updates in the field of cryptography and cybersecurity.