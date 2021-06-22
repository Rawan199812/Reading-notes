## JSON Web Tokens 

***How do JSON Web Tokens work?***
**In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. In general, you should not keep tokens longer than required.**


- Whenever the user wants to access a protected route or resource, the user agent should send the JWT, typically in the Authorization header using the Bearer schema.

***In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are:***
- Header
- Payload
- Signature

**Header** 
- The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.

**Public claims: These can be defined at will by those using JWTs. But to avoid collisions they should be defined in the IANA JSON Web Token Registry or be defined as a URI that contains a collision resistant namespace.**

**Private claims: These are the custom claims created to share information between parties that agree on using them and are neither registered or public claims.**