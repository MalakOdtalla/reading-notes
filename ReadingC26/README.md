## JSON Web Token

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

## When should you use JSON Web Tokens?

- Authorization: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.

- Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties.

## Why JWT?
Instead of storing information on the server after authentication, JWT creates a JSON web token and encodes, sterilizes, and adds a signature with a secret key that cannot be tampered with. This key is then sent back to the browser. Each time a request is sent, it verifies and sends the response back.

The main difference here is that the user’s state is not stored on the server, as the state is instead stored inside the token on the client-side.

JWT also allows us to use the same JSON Web Token in multiple servers that you can run without running into problems where one server has a certain session, and the other server doesn’t.