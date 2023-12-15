## Class 15 Notes

### OAuth

1. **What is OAuth?**

    - OAuth is an open standard for access delegation, frequently used as a way for users to grant website or applications access to information without providing their credentials.

2. **Give an example of what using OAuth would look like.**

    - Whenever I try to login to my mobile game I can either use my own username and password or use my Google account to authenticate myself which allows me access to my game.

3. **How does OAuth work? What are the steps that it takes to authenticate the user?**

    - **Request Authorization:** The app requests permission from the user to access resources.

    - **User Approval:** The user grants the app permission to access their resources.

    - **App Receives Authorization Grant:** The app receives an authorization grant which is a credential representing the user's authorization.

    - **App Requests Access Token:** The app exchanges the authorization grant for an access token.

    - **Authorization Server Authenticates and Issues Token**: The authorization server authenticates the app and issues an access token.

    - **Access Token Used for API Access:** The app uses the access token to access the user's resources from the resource server.

    >- **Source: ChatGPT**

4. **What is OpenID?**

    - It's an authentication layer built on top of OAuth.  Its focused on user authentication and is used to log in to websites using information form another website.

### Authorization vs Authentication

1. **What is the difference between authorization and authentication?**

    - Authentication is the process of verifying who a user is via login procedures.
    - Authorization is the process of verifying what specific applications and data the user has access to.

2. **What is Authorization Code Flow?**

    - The Authorization Code Flow is a method of exchanging an authorization grant for an access token.

3. **What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**

    - PKCE extends the Authorization Code flow to be used with public clients.  It enchances security by generating a token on the client side which is verified by the authorization server.

4. **What is Implicit Flow with Form Post?**

    - Implicit flow is where a access token is returned immediately without an extra authorization code exchange step. This is considered less secure and no longer recommended.

5. **What is Client Credentials Flow?**

    - This flow is the application itself is the owner and authenticates directly to the authorization server to get an access token.

6. **What is Device Authorization Flow?**

    - This flow is used for devices that don't have a web browser or operate in limited input capabilities. This involves verifying the user on a seperate device that has better capabilities.  

7. **What is Resource Owner Password Flow?**

    - This less secure flow allows the user to provide their service credentials (username and password) directly to the application, which uses them to obtain an access token. This bypasses the need for the user to authorize the application but exposes the credentials to the application.