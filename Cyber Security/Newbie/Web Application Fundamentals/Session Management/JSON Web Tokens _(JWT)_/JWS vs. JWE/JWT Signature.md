The JWT signature is the third part of a JSON Web Token (JWT) and is used to verify the integrity of the token. The signature is calculated using a secret key or a public/private key pair, depending on the algorithm used.

To create the signature, the signing algorithm takes the encoded header and payload as inputs and generates a digital signature. The signature is then appended to the encoded header and payload to form the complete JWT.

When the JWT is received by a party that needs to verify the signature, the same algorithm is used to recalculate the signature using the same secret key or public key. If the recalculated signature matches the signature in the token, the token is considered valid.

The algorithm used to calculate the signature is specified in the "alg" parameter of the JWT header. Some common signature algorithms used with JWTs include:

- HMAC with SHA-256 (HS256): This algorithm uses a secret key to sign and verify the token. The secret key must be kept secret by the parties involved in the exchange.  
- RSA with SHA-256 (RS256): This algorithm uses a public/private key pair to sign and verify the token. The signer signs the token with their private key, and the verifier verifies the signature using the signer's public key.  
- ECDSA with SHA-256 (ES256): This algorithm uses an elliptic curve digital signature algorithm to sign and verify the token. The signer signs the token with their private key, and the verifier verifies the signature using the signer's public key.  

It is important to keep the secret key or private key secure and to verify the signature of the token to ensure that the token has not been tampered with or created by an unauthorized party.