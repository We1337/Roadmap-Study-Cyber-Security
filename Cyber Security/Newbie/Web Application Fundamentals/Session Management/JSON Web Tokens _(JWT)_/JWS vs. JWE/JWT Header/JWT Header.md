The JWT header is a JSON object that describes the format and signing algorithm used for a JSON Web Token (JWT). It consists of two parts: the "alg" (algorithm) parameter, which identifies the signing algorithm used to sign the JWT, and the "typ" (type) parameter, which specifies the type of token.

Here is an example of a JWT header:

```
{
  "alg": "HS256",
  "typ": "JWT"
}
```

In this example, the "alg" parameter specifies that the HMAC SHA-256 algorithm is used to sign the JWT, while the "typ" parameter specifies that the token is a JWT.

The "alg" parameter can take various values depending on the signing algorithm used, such as "HS256" for HMAC-SHA256, "RS256" for RSA-SHA256, or "ES256" for ECDSA with SHA-256. The "typ" parameter is usually set to "JWT" to indicate that the token is a JSON Web Token.

The header is Base64url encoded and included as the first part of the JWT, followed by the payload and signature. When the JWT is received by the server, the header is decoded and the "alg" parameter is used to determine the algorithm used to verify the signature.