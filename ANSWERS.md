<!-- Answers to the Short Answer Essay Questions go here -->

1.  Describe Middleware, Sessions (as we know them in express), bcrypt and JWT.

    Middleware are functions, 3rd party or custom, that execute between the request and the request handler. Middleware in express is flexible, has access to the req/res objects, and is stored in a queue/stack.

    Sessions are objects (req.sessions) that hold data across requests and is unique for each user. Sessions also allow applications hold state as users perform actions.

    Bcrypt is a 3rd party library used to protect passwords by hashing and adding a salt to them. Furthermore bcrypt allows devs to increase the "cost" which is the parameter that refers to the number of iterations performed by the hashing algorithm to expand a key. Bcrypt effectively prevents rainbow attacks and brute force attacks.

    JWT is an industry standard for token authentication and is available for use as a 3rd party library in express. JWTs are more secure than cookies, transmitted quickly, and self-contained so querying database is not needed.

2.  What does bcrypt do in order to prevent attacks?

    Bcrypt hashes passwords and also adds a salt to them. It also increases the time it takes to generate passwords by hackers via a "cost" parameter.

3)  What are the three parts of the JSON Web Token?

    3 parts of the JWTs are the header, payload, and signature.

    The header includes the type of token and the hashing algorithm used.

    The payload uses to store data and the signature is the hashed string that includes the header, payload, and secret.
