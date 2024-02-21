## Class 33 Notes

1. **What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?**

- **Primary Purpose of JSON Web Tokens (JWTs)**

    - JSON Web Tokens (JWTs) are a compact, URL-safe means of representing claims to be transferred between two parties. The primary purposes of JWTs include:

        - **Authentication:** After a user logs in, the server creates a JWT for that user, which is then stored client-side (typically in local storage or cookies) and included in subsequent requests to the server. The server then verifies the token to identify the user and provide access to protected resources.

        - **Information Exchange:** JWTs can securely transfer information between parties as JSON objects. Because JWTs can be signed—either using a secret (with the HMAC algorithm) or a public/private key pair (with RSA or ECDSA)—the receiver can verify the sender's identity and ensure the data hasn't been tampered with.

- **How JWTs Work: Encoding and Decoding Data**

    - JWTs consist of three parts: Header, Payload, and Signature, each separated by a dot (.).

        - **Header:** Typically consists of the token type (JWT) and the signing algorithm being used, such as HMAC SHA256 or RSA.

        - **Payload:** Contains the claims, which are statements about an entity (typically the user) and additional data. These claims can be registered claims, public claims, and private claims.

        - **Signature:** Created by taking the encoded header, the encoded payload, a secret, and the algorithm specified in the header.

        - **Encoding:** When a JWT is created, the Header and Payload are encoded with Base64Url and then concatenated with a dot. This string is then signed with the Header's specified algorithm using a secret or a private key. The resulting signature is appended to the encoded string, forming the final JWT.

        - **Decoding:** To decode a JWT, the recipient splits the token by dots to retrieve the Header and Payload, which are Base64Url decoded. The Signature is verified using the Header's specified algorithm and the secret or public key. If the verification is successful, the Payload can be trusted and used.

2. **How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?**

    - **JWT Authentication with Django REST Framework**
        - Django REST Framework (DRF) supports JWT authentication to secure API endpoints. Integrating JWT authentication involves several key components:

            - **JWT Authentication Class:** DRF allows the use of custom authentication classes. By specifying a JWT authentication class, you can configure your APIs to authenticate requests using JWTs.

            - **Token Generation and Validation:** Upon successful authentication (e.g., username and password), a JWT is generated and returned to the user. This token must then be included in the Authorization header of HTTP requests. DRF's JWT authentication class is responsible for validating the token in each request.

            - **User Identification:** The validated token is used to identify the user making the request, allowing DRF to apply permissions and access controls as configured.

3. **Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?**

    - Django’s built-in server (runserver) is intended for development purposes only due to several reasons:

        - **Performance:** It is not optimized for performance and can't handle real-world traffic loads efficiently.

        - **Security:** Lacks security features necessary to protect against attacks in a production environment.

        - **Reliability:** Does not have the reliability features required for a production server, such as process management and load balancing.

    - **Alternative Server Options for Django Applications**
    
        - For deploying a Django application in production, consider using a more robust web server. Some popular options include:

            - **Gunicorn:** A Python WSGI HTTP Server for UNIX, it's easy to use, supports worker processes, and is widely used in conjunction with Nginx.

            - **uWSGI:** A project aiming at developing a full stack for building hosting services, uWSGI is another popular choice that supports WSGI, with Nginx often used as a reverse proxy.

            - **Daphne:** An HTTP, HTTP2, and WebSocket protocol server for ASGI and ASGI-HTTP, suitable for Django Channels.