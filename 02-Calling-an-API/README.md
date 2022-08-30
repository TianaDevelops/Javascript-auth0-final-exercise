# Sample 02 - Calling an API

This app demonstrates how to log in using the Auth0 Universal Page, and call a backend API using an access token.

## Installation

After cloning the repository, run:

```bash
$ npm install
```

This will install all of the necessary packages in order for the sample to run.

## Running the Application

To start the app from the terminal, run:

```bash
$ npm run dev
```

Open the application in the browser at [http://localhost:3000](http://localhost:3000).


## Setting up your API

Open the APIs in the browser at [https://manage.auth0.com/dashboard/us/dev-dyur1scc/apis/630e09eb2899e980083ce7c3/quickstart]
1. Choose a JWT library
As your API will be parsing JWT formatted access tokens, you will need to setup these capabilities on your API.

You can navigate to jwt.io and choose from there. Remember to pick a library that support your selected signing algorithm.

2. Configuring your API to accept RS256 signed tokens

Configure the library that will validate the access tokens in your API. Validating a token means that you are certain you can trust its contents.

## Restricting Access to Managers Only - Using RBAC
3. Define Permissions and manage Authorization Policies
On the Permissions tab, you can define what scopes this API may accept. 

On the Settings tab, enable Authorization Policy Enforcement for your API. If enabled, only Roles and Permissions assigned to your user will be included in the token.

That's it!

## Adding the API to your application
Go to your Auth0 dashbaord and go to the Application

Click the API tab and add slide over the slider to Authorize your new API to access this application.


## Setting up/confirming Manager Access
Go to your Auth0 dashbaord and go to User Management > Roles

Create a role called "Manager"

## Adding Managers to role
Switch to the Users tab and click Add Users

## Frequently Asked Questions

We are compiling a list of questions and answers regarding the new JavaScript SDK - if you're having issues running the sample applications, [check the FAQ](https://github.com/auth0/auth0-spa-js/blob/master/FAQ.md)!

## What is Auth0?

Auth0 helps you to:

- Add authentication with [multiple authentication sources](https://docs.auth0.com/identityproviders), either social like **Google, Facebook, Microsoft Account, LinkedIn, GitHub, Twitter, Box, Salesforce, among others**, or enterprise identity systems like **Windows Azure AD, Google Apps, Active Directory, ADFS or any SAML Identity Provider**.
- Add authentication through more traditional **[username/password databases](https://docs.auth0.com/mysql-connection-tutorial)**.
- Add support for **[linking different user accounts](https://docs.auth0.com/link-accounts)** with the same user.
- Support for generating signed [Json Web Tokens](https://docs.auth0.com/jwt) to call your APIs and **flow the user identity** securely.
- Analytics of how, when and where users are logging in.
- Pull data from other sources and add it to the user profile, through [JavaScript rules](https://docs.auth0.com/rules).

## Create a free Auth0 account

1. Go to [Auth0](https://auth0.com/signup) and click Sign Up.
2. Use Google, GitHub or Microsoft Account to login.

## Issue Reporting

If you have found a bug or if you have a feature request, please report them at this repository issues section. Please do not report security vulnerabilities on the public GitHub issue tracker. The [Responsible Disclosure Program](https://auth0.com/whitehat) details the procedure for disclosing security issues.

## Author

[Auth0](auth0.com)

## License

This project is licensed under the MIT license. See the [LICENSE](LICENSE.txt) file for more info.
