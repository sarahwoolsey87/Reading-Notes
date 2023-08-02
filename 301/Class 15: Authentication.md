# Authentication

[What is OAuth?](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

## What is OAuth?

OAuth (Open Authorization) is an open standard protocol that allows secure authorisation and access delegation for applications, websites, or services to interact with a user's resources on another website or service without sharing the user's credentials. It is commonly used to enable single sign-on (SSO) functionality and grant limited access to a user's data on third-party platforms.

## Give an example of what using OAuth would look like.

Consider a scenario where a user wants to sign up for a new fitness app using their Google account. The fitness app uses OAuth to request access to the user's basic profile information (like name and email) from their Google account. Instead of the user sharing their Google account credentials with the fitness app, they are redirected to Google's authentication page, where they can log in securely. Once the user grants permission, the fitness app receives an access token from Google, which allows it to access the user's basic profile information.

## How does OAuth work? What are the steps that it takes to authenticate the user?

How OAuth works and the steps involved:

- **Authorisation Request:** When a user wants to grant a third-party application access to their resources (e.g., profile information, photos, etc.), the application initiates an authorisation request by redirecting the user to the authorization server (e.g., Google, Facebook) with specific authorisation parameters.

- **User Authentication:** The user is redirected to the authorisation server's login page, where they are required to log in and provide their credentials to the server.

- **User Consent:** After successful authentication, the authorisation server presents the user with a consent screen that outlines the data the third-party application is requesting access to. The user can choose to grant or deny access to their data.

- **Authorisation Grant:** If the user consents, the authorisation server generates an authorisation code or access token, depending on the OAuth flow used.

- **Token Exchange:** The third-party application uses the authorisation code or access token obtained from the authorisation server to request an access token and refresh token (if applicable). The access token allows the application to access the user's resources on the server for a limited time.

- **Access Resources:** With the access token, the third-party application can securely access the user's resources on the server (e.g., retrieve profile information or perform actions on their behalf).

- **Refresh Tokens (optional):** If the authorisation flow includes refresh tokens, the third-party application can use them to obtain new access tokens without requiring the user's direct involvement, allowing for longer-term access.

## What is OpenID?

OpenID is another open standard authentication protocol that works in conjunction with OAuth. While OAuth focuses on authorisation and access delegation, OpenID is primarily focused on authentication and user identity verification. It allows users to log in to multiple websites or applications using a single set of credentials, providing a single sign-on (SSO) experience.

In an OpenID flow, the user's identity provider (IdP) authenticates the user and then shares their identity information with the relying party (RP), which is the website or application the user wants to access. OpenID Connect (OIDC) is a popular implementation of OpenID, which combines the capabilities of OpenID and OAuth to provide a robust and secure authentication mechanism.

[Authorisation & Authentication Flows](https://auth0.com/docs/flows)

## What is the difference between authorisation and authentication?

Authorisation and authentication are both critical aspects of security and access control, but they serve different purposes:

- **Authentication:** Authentication is the process of verifying the identity of a user or entity. It ensures that the user is who they claim to be. Authentication is typically done by presenting credentials such as username and password, biometrics, or using other authentication methods like multi-factor authentication (MFA).

- **Authorisation:** Authorisation is the process of determining what actions or resources a user or entity is allowed to access after they have been authenticated. It defines the permissions and privileges granted to the user based on their identity and role. Authorisation is about granting or denying access to specific resources or functionalities.

## What is Authorisation Code Flow?

The Authorisation Code Flow is an OAuth 2.0 flow designed for web applications that can securely maintain a client secret. It is considered more secure than other OAuth flows because it separates the client credentials from the user's access token.

In this flow:

The client (web application) initiates the authorisation request and redirects the user to the authorisation server.

The user authenticates with the authorisation server and gives consent to the client's access request.
The authorization server sends an authorisation code back to the client's redirect URL.
The client exchanges the authorisation code for an access token and, optionally, a refresh token through a secure server-to-server request.

## What is Authorisation Code Flow with Proof Key for Code Exchange (PKCE)?

PKCE is an extension to the Authorisation Code Flow and is used to enhance the security of the authorisation process, especially for mobile and native applications that cannot securely store a client secret.

In this flow, the client dynamically creates a "code_verifier" and a "code_challenge" and includes the "code_challenge" in the authorisation request. The authorisation server requires the client to present the original "code_verifier" when exchanging the authorisation code for an access token. This ensures that even if the authorisation code is intercepted during the redirect, an attacker cannot exchange it for an access token without the original "code_verifier."

## What is Implicit Flow with Form Post?

The Implicit Flow with Form Post is an OAuth flow primarily designed for JavaScript-based single-page applications (SPAs) that cannot maintain a client secret. In this flow, the access token is returned directly to the client-side through the URL fragment or hash. To enhance security and avoid exposing sensitive information in the browser history, the access token is returned in a hidden form field via a form post to the client-side.

## What is Client Credentials Flow?

The Client Credentials Flow is an OAuth flow used by confidential clients (such as web servers and backend services) to obtain an access token without user involvement. The client directly exchanges its own credentials (client ID and client secret) with the authorisation server for an access token. This flow is appropriate when the client is acting on its behalf rather than on behalf of a specific user.

## What is Device Authorisation Flow?

The Device Authorisation Flow is designed for devices with limited input capabilities, such as smart TVs or Internet of Things (IoT) devices. In this flow, the device displays a user code and instructs the user to visit a specific URL on another device to complete the authentication process. The user enters the code on the second device and completes the authentication, after which the original device can obtain the access token.

## What is Resource Owner Password Flow?

The Resource Owner Password Flow (ROPC) allows trusted applications to directly obtain an access token from the authorisation server using the user's credentials (username and password). This flow should be used with caution and only in specific situations, as it requires the client to handle the user's credentials directly, which might raise security concerns. It is generally recommended to use more secure flows like the Authorisation Code Flow or Implicit Flow when possible.

[AuthO for Single Page Apps](https://auth0.com/docs/libraries/auth0-react)