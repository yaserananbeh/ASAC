# Class-11


## What is OAuth?
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.
## Give an example of what using OAuth would look like.
The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.
## How does OAuth work? What are the steps that it takes to authenticate the user?
Let’s assume a user has already signed into one website or service (OAuth only works using HTTPS). The user then initiates a feature/transaction that needs to access another unrelated site or service. The following happens (greatly simplified):

- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
- The first site gives this token and secret to the initiating user’s client software.
- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
- The user approves (or their software silently approves) a particular transaction type at the first website.
- The user is given an approved access token (notice it’s no longer a request token).
- The user gives the approved access token to the first website.
- The first website gives the access token to the second website as proof of authentication on behalf of the user.
- The second website lets the first website access their site on behalf of the user.
- The user sees a successfully completed transaction occurring.
    OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

## What is OpenID?
ID allows you to use an existing account to sign in to multiple websites, without needing to create new passwords.


## What is the difference between authorization and authentication?
Authentication confirms that users are who they say they are. Authorization gives those users permission to access a resource.
## What is Authorization Code Flow?
- The user clicks Login within the regular web application.

- Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint).

- Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

- The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the regular web application.

- Your Auth0 Authorization Server redirects the user back to the application with an authorization code, which is good for one use.

- Auth0's SDK sends this code to the Auth0 Authorization Server (/oauth/token endpoint) along with the application's Client ID and Client Secret.

- Your Auth0 Authorization Server verifies the code, Client ID, and Client Secret.

- Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

- Your application can use the Access Token to call an API to access information about the user.

- The API responds with requested data.
## What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
- The user clicks Login within the application.

- Auth0's SDK creates a cryptographically-random code_verifier and from this generates a code_challenge.

- Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) along with the code_challenge.

- Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

- The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the application.

- Your Auth0 Authorization Server stores the code_challenge and redirects the user back to the application with an authorization code, which is good for one use.

- Auth0's SDK sends this code and the code_verifier (created in step 2) to the Auth0 Authorization Server (/oauth/token endpoint).

- Your Auth0 Authorization Server verifies the code_challenge and code_verifier.

- Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

- Your application can use the Access Token to call an API to access information about the user.

- The API responds with requested data. 
## What is Implicit Flow with Form Post?
As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication.
## What is Client Credentials Flow?
With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don't make sense. Instead, M2M apps use the Client Credentials Flow (defined in OAuth 2.0 RFC 6749, section 4.4).
## What is Device Authorization Flow?
With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. To do this, device apps use the Device Authorization Flow (drafted in OAuth 2.0). For use with mobile/native applications.
## What is Resource Owner Password Flow?
Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form. The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.
