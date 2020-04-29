# Class12 - OAuth Authentication - 4/28/2020

## What is OAuth
* an open standard for access delegation.
* serves as a way to give users the ablity to grant application access to services

## How does it work?
* application developers needs to register the application on Github OAuth and get client_id and client_secret etc.
* application developers use client_id and client_secret and designated github url and other information to make an url that redirect the users to github sign in page.
* when user sign in with their github credential, there are several handshake happens:
  1. github authenticates user's credential, upon successful it would send application with one-time-use code.
  2. application server acts as client and use this one-time-use code to make post request with required information to github.
  3. github responds with a token that give access to user's certain github information to the application server.
  4. application server acts as client and use this token to make get request to github to get user's certain github information.
  5. github responds with requested user's github information to the application server.
  6. application server grabs username and generates hashed password for this username and save those credential to the database. Then server generates an application token based on user credential and send it to user for future authentication.

## Security Concerns
* it is possible that developers with bad intention make a mockup service sign-in page and redirect users to that page upon sign-in and steal their credentials
* it is possible that develpers with bad intention manipulate the scope and get extra user's information that is not necessary for the application.