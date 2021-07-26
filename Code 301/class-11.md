#### What is OAuth?
- open standard authorization protocol
- thrid party authorization
#### Give an example of what using OAuth would look like.
- when you log onto a website and it offers you to sign in using various options – Facebook, Google, Github – and it redirects you to that website for you to sign in from
#### How does OAuth work? What are the steps that it takes to authenticate the user?
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. 
6. After authentication, the client is asked to approve the authorization transaction to the second website.
7. The user approves (or their software silently approves) a particular transaction type at the first website.
8. The user is given an approved access token (notice it’s no longer a request token).
9. The user gives the approved access token to the first website.
10. The first website gives the access token to the second website as proof of authentication on behalf of the user.
11. The second website lets the first website access their site on behalf of the user.
12. The user sees a successfully completed transaction occurring.
#### What is OpenID?
- security service for "humans to log into machines" whereas OAuth is "machines logging into machines for humans"

---

#### What is the difference between authorization and authentication?
- Authenticaion: process of verifying who a user is
- Authorization: process of verifying what they have access to
#### What is Authorization Code Flow?
- user logs in by having the Authorization Code exchanged for a token
#### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
- user logs in by having the Authorization Code with a Proof Key, without which it cannot be exchanged for a token
#### What is Implicit Flow with Form Post?
- using OpenID Connect, it implements a web sign-in by requesting and objtaining tokens through the front channel without secrets or backend calls
#### What is Client Credentials Flow?
- user passes Client ID and Client Secret to authenticate themselves and get a token
#### What is Device Authorization Flow?
- device apps use this to pass along their Client ID to initiate the authorization process and get a token
#### What is Resource Owner Password Flow?
- users provide credentials (username and password) through an interactive form
