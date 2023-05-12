The JWT payload is the second part of a JSON Web Token (JWT) and contains the claims that provide information about the entity (typically a user) and additional data related to the token itself. The payload is a JSON object that consists of one or more name-value pairs, called claims.

There are three types of claims that can be included in the JWT payload:

1. Registered claims: These are a set of predefined claims that are recommended to be used to provide information about the token itself or the user. Some examples of registered claims include "iss" (issuer), "sub" (subject), "aud" (audience), "exp" (expiration time), and "iat" (issued at time). These claims have standardized meanings and their values should be respected by all parties using the token.
2. Public claims: These are custom claims defined by the parties that exchange the token. They are used to provide additional information about the entity or the context of the token. Public claims should be defined in a way that avoids collisions with other claim names.
3. Private claims: These are custom claims that are specific to a particular application or organization. They are used to convey information that is relevant only to the parties that exchange the token. Private claims should be defined using a namespace that is unlikely to clash with other claim names.

Here is an example of a JWT payload containing a set of registered claims:

```
{
  "iss": "https://example.com",
  "sub": "1234567890",
  "name": "John Doe",
  "iat": 1516239022,
  "exp": 1616239022
}
```

In this example, the payload contains the "iss" (issuer) claim, which identifies the entity that issued the token, the "sub" (subject) claim, which identifies the entity associated with the token, the "name" claim, which provides the name of the user, and the "iat" (issued at time) and "exp" (expiration time) claims, which indicate the times when the token was issued and when it expires.