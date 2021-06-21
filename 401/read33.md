# What is JSON Web Token?
 JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

## When should you use JSON Web Tokens?
 Here are some scenarios where JSON Web Tokens are useful:

 - Authorization: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

 - Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with.

## How do JSON Web Tokens work?
 In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. In general, you should not keep tokens longer than required.

# How to Use JWT Authentication with Django REST Framework
 JWT stand for JSON Web Token and it is an authentication strategy used by client/server applications where the client is a Web application using JavaScript and some frontend framework like Angular, React or VueJS.

 In this tutorial we are going to explore the specifics of JWT authentication. If you want to learn more about Token-based authentication using Django REST Framework (DRF), or if you want to know how to start a new DRF project you can read this tutorial: How to Implement Token Authentication using Django REST Framework. The concepts are the same, we are just going to switch the authentication backend. 

 The JWT is acquired by exchanging an username + password for an access token and an refresh token.

 The access token is usually short-lived (expires in 5 min or so, can be customized though).

 The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again.