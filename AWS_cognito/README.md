# AWS Cognito

*Built by LATAM Team*

**Supports:** *iOS and Android*
*Current Version: 0.0.19 iOS, 0.0.1 Android*

 
## About

Amazon Cognito lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily.

## What needs does it meet?
### Cloud Based User Database
Clients can generate a user data base without on-site infraestructure.

### Scale up
All concurrency at login point is hanlded and scale automatically by the AWS Infraestructure

### Free tier
Up to 50,000 Monthly Active Users wihtout any cost.

### When to use?

- Client doesn't have an own user database.
- Cost effective solution.
- Controlled access to the application or sections of it.
- Scalability.

## Analytics

- Firebase to be added.
- Amazon Pinpoint can be activated through AWS console.

## Related Technologies

Social Login. To be implmented as part of the second face integration.

## Configuration

Previous to configure the plugin the client needs to have a AWS account and a User Pool created on AWS Cognito.

The userpool should have been configured using a client secret. 

Add the plugin ""AWS Cognito Login" to your app, through the zapp gallery.

![image\_2][image-2]

Provide the following parameters to configure the User Pool in the plugin configuration:

- clientID
- cleintSecret
- Region
- userpoolid

*Region should cosider the following values in iOS:*
- useast1
- useast2
- uswest1
- uswest2
- euwest1
- euwest2
- eucentral1
- apsoutheast1
- apnortheast1
- apnortheast2
- apsoutheast2
- apsouth1
- saeast1
- cnnorth1
- cacentral1
- usgovwest1
- cnnorthwest1
- euwest3
- usgoveast1
- eunorth1
- apeast1

![image\_3][image-3]

The plugin can be personalized to fit a client's corporative image. A sketch file is hosted as part of the documentation; all keys for texts, colors and components are there and with clear visuals.

[Sketch file](https://github.com/applicaster/latam-product-documentation/blob/master/AWS_cognito/cognito.sketch)

![image\_1][image-1]

All keys described in the file are available in the plugin configuration.

![image\_4][image-4]


The plugin covers the following flows:

- User Sign In
- User Sign Up
- User Forgot Password
- User activation

### Out of scope

For registration the plugin takes the following fields only:

- Username
- E-mail
- Password

AWS cognito supports by default user attributes defined in the [OpenID Connect Specification](https://openid.net/specs/openid-connect-core-1_0.html#StandardClaims)

For following phases the development should explore a dynamic way to define which fields to show as part of the registration.

### Next Phases

- Identity Pools (Fedarated Entities). Specifically social login.
- "Not now" Flow. Suggest to login for clients who chose to add this type of suggestion to improve app experience.
- Dynamic resgistration fields.
- Firebase Analytics.


[image-1]:	https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/AWS_cognito/ss_1.png
[image-2]:	https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/AWS_cognito/ss_2.png
[image-3]:	https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/AWS_cognito/ss_3.png
[image-4]:	https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/AWS_cognito/ss_4.png
