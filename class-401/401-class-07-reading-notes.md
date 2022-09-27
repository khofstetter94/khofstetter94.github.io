# Bearer Authorization

[Intro to JWT](https://jwt.io/introduction/)

- What is a JSON Web Token (JWT)?
  - JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
- When should we use JSON Web Tokens?
  - Authorization: the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.
  - Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with.
- Claims are expected in which structural component of a JWT?
  - The payload

[Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)

- If I get a JWT and I can decode the payload, how can we call that secure?
  - JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.
- If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.
  - The calculated Hash(payload + secret)
- Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.
  - "Let's assume Alice wants to send a JWT to Bob. They both know some shared secret. Mallory doesn't know that secret, but wants to interfere and change the JWT. To prevent that, Alice calculates Hash(payload + secret) and appends this as signature.When receiving the message, Bob can also calculate Hash(payload + secret) to check whether the signature matches. If however, Mallory changes something in the content, she isn't able to calculate the matching signature (which would be Hash(newContent + secret)). She doesn't know the secret and has no way of finding it out. This means if she changes something, the signature won't match anymore, and Bob will simply not accept the JWT anymore."

[JWTS Explained](https://www.youtube.com/watch?v=926mknSW9Lo)

- Why use JWT?
  - It is used to securely transfer information between any two bodies and it is digitally signed which means the information is verified and trusted.
- JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.
  - JWT is so compact that is can be sent to another user with the URL, POST request, or HTTP Header, which in turn makes it a fast transmission. Being self-contained means it contains information about the user which in turn avoids querying the database more than once. Logging in once will give you a token and any other time you want to sign in, the token will just be verified and the information will be given.
- What are the three components (the structure) of a JWT signature?
  - 'aaaaaaaa.bbbbbbbb.cccccccc'
    - The 'a' part: is the header, JSON object that includes "{ "alg": "HMAC" or " SHA256" or "RSA", "typ": "JWT"}"
    - The 'b' part: is the payload, contains the claims (user details or additional metadata) in the form on a JSON object
    - The 'c' part: is the signature, uses base64 encoded header with the base64 encoded payload along with the secret. All of which is put through HMACSHA256 encoding.

## Things I want to know more about

- Creating the JWT signature. The differences between HMAC, SHA256, and RSA.

[Return home](https://khofstetter94.github.io/reading-notes/)

