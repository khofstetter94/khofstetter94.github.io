# Authentication

- [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

- [Authorization and Authentication flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow)

- **What is OAuth?** - OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.
- **Give an example of what using OAuth would look like.** - logging into a website and clicking the button that says "login with Google" or "login with Facebook"
- **How does OAuth work? What are the steps that it takes to authenticate the user?** -

        1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
        2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
        3. The first site gives this token and secret to the initiating user’s client software.
        4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
        5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
        6. The user approves (or their software silently approves) a particular transaction type at the first website.
        7. The user is given an approved access token (notice it’s no longer a request token).
        8. The user gives the approved access token to the first website.
        9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
        10. The second website lets the first website access their site on behalf of the user.
        11. The user sees a successfully completed transaction occurring.
        12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

- **What is OpenID?** - OpenID is about authentication, OpenID is for humans logging into machines

- **What is the difference between authorization and authentication?** - Authentication  proves the user is who they say they are and authorization gives permission or authority
- **What is Authorization Code Flow?** - exchanging an Authorization Code for a token.
- **What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?** - The PKCE-enhanced Authorization Code Flow introduces a secret created by the calling application that can be verified by the authorization server; this secret is called the Code Verifier. Additionally, the calling app creates a transform value of the Code Verifier called the Code Challenge and sends this value over HTTPS to retrieve an Authorization Code.
- **What is Implicit Flow with Form Post?** - Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls.
- **What is Client Credentials Flow?** - M2M apps use the Client Credentials Flow in which they pass along their Client ID and Client Secret to authenticate themselves and get a token.
- **What is Device Authorization Flow?** - Device apps use the Device Authorization Flow in which they pass along their Client ID to initiate the authorization process and get a token.
- **What is Resource Owner Password Flow?** - Requests that users provide credentials (username and password), typically using an interactive form.

## Things I want to know more about

- OAuth.. pretty much everything discussed in the reading

[Return home](https://khofstetter94.github.io/reading-notes/)
