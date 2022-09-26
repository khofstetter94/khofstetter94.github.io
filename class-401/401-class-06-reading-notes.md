# Authentication

[Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

- Explain to a non-technical friend how you would safely hash and store a password.
  - In order to hash your password, you would put the plain text through an algorithm that changes the characters into something unreadable. This unrecognizable string is then stored.
- What is Bcrypt?
  - Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.
- Why might you use something like Bcrypt?
  - Even with hashin, passwords aren't safe from attacks, we need algorithms which can make the brute force attacks slower and minimize the impact

[Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)

- What is Basic Authentication?
  - basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.
- What properties are necessary in the header of a Basic Auth request?
  - Authorization: Basic \<credentials>
- How are username:password in Basic Auth encoded?
  - The username and password are combined with a single colon (:). This means that the username itself cannot contain a colon.
  - The resulting string is encoded into an octet sequence. The character set to use for this encoding is by default unspecified, as long as it is compatible with US-ASCII, but the server may suggest use of UTF-8 by sending the charset parameter.[9]
  - The resulting string is encoded using a variant of Base64 (+/ and with padding).
  - The authorization method and a space (e.g. "Basic ") is then prepended to the encoded string.

[OWASP Auth Cheatsheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

- Define the authentication process to a non-technical recruiter.
  - Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.
- How should your error messaging respond (both HTTP and HTML)? Why?
  - Using any of the authentication mechanisms (login, password reset or password recovery), an application must respond with a generic error message regardless of whether:
    - The user ID or password was incorrect.
    - The account does not exist.
    - The account is locked or disabled.
  - The objective is to prevent the creation of a discrepancy factor, allowing an attacker to mount a user enumeration action against the application.
- Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.

## Things I want to know more about

- Hashing a password and creating proper error messaging responses.

[Return home](https://khofstetter94.github.io/reading-notes/)
