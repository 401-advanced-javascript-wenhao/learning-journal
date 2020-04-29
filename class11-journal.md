# Class11 - Basic Authentication - 4/27/2020

## How does basic authorization and basic authentication work
1. Sign up process
  * User credential (username and password) send it to server.
  * Hash algorithm generates hashed password and save it to the database. Hash algorithm is one-way, it is impossible to get the original password from hashed password.
  * Server would generate a token and send it to user for future authentication.
2. Sign in process
  * User credential is encryped (base64) and added to request authorization header and send it to server.
  * Authentication middleware captures request authorization header and decrypt (base64) user credential.
  * Hash algorithm compares decrypted password with this user's hashed password stored in the database.
  * If authentication is successful, server would generate a token and send it to client for future authentication.
  * If authentication is not successful, server would send authentication error to the user.