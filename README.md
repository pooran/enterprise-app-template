# Enterprise App Template
From my past experience of building, rearchitecting enterprise apps for various domains and industry verticals, I am attempting to create a template that takes care of most of the necessary flows to build a truly scalable enterprise app template

1. Authentication
2. Authorization
3.  

## Authentication

Today world is moving towards passwordless multi factor authentication. Come to think of it, having username password kind of infra, needs many screens and complexities to manage
1. Password complexity regex
2. Reset password every x days
3. MFA is kind of mandatory in most scenarios
4. forgat password - verify be email - another page/screen for reset password 

### What are the alternatives

#### Simplest one is MagicLink

1. Collect Email
2. Send Email with Unique Link
3. User Opens Email and Clicks Link
4. User is now authenticated

#### Others are Multi Auth Managers

Especially when one is building an enterprise app, we have to work with customers who have their own SSO/AD/SCIM/OAuth/OpenId/SAML implemnentations along with custom MFA like SMS/OTP/Authenticator/KeyFob etc. We cannot just expect them to throw that to wind and ask them to create an email and password on our server.

There are many providers who help enterprise adoption faster

1. OpenAM - https://www.openidentityplatform.org/openam
2. WorkOS - https://workos.com/
3. AWS Congito - https://aws.amazon.com/cognito/


## Authorizations

After user is authenticated what next? What 


