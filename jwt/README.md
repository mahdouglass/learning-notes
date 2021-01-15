# JWT

 - **JWT** - JSON Web Token, open standard for creating and transmitting data
 - A cryptographically signed token (also called a digital signature)
 - Verify payload's authenticity and integrity
 - Encrypt JSON payload to provide confidentiality

 ## Cryptographically Signed Token

 - Are issued by server to a user, then is presented by user back to the server to prove authorization (like a handshake to prove identification)
 - Server knows secret key and only server can issue valid tokens
 - Can't modify token and its JSON payload without detection

 ## Token Structure

 - A signed JSON web token has a header, JSON payload, and the signature

### Header

- Contains JSON that identifies the encryption algorithm which generates the signature (can contain other information)

### Payload

- A JSON object that defines the claims (there are 7 standard claims). The claims store information like user's identity, expiration information, issuer, etc.

### Signature

- Created by encoding the header and payload with base64. Then the server will encrypt the base64 string using it's private key. It can later verify by comparing the token received to the token's signature block.

## Benefits

- JSON is a great choice for storing authentication information and works with a lot of languages
- JWT claims allows for easily stored additional information that can be accessed within the application without needing a database
- Tokens are small and URL-safe, can be stored as local/session cookies
- A lot of common web frameworks use JWT

## Downsides

- JWT is used for authorization (determines if a user is allowed to perform after authentication) not authentication (ensuring user is who they say they are). 
