
# Adobe Primetime Authentication 

*Built by LATAM Team*

**Supports:** *iOS, Android, Android TV, tvOS, FireTV and Roku*

**Current Versions:**
- *5.0.0 (iOS)*
- *0.0.3 (Android)*
- *0.3.0 (tvOS)*
- *0.1.18 (Android TV)*
- *0.1.18 (FireTV)*
- *0.1.0 (Roku)*
 
*Note: AndroidTV and FireTV share the same plugin*

## About

Adobe Primetime Authentication is a hosted service that serves as a proxy between programmers and MVPD's. It verifies users entitlement to content based on their TV Subscription.


### What needs does it meet?

- Authentication, authorization and logout.
- Levels of entitlement.
- Seamless integration to MVPD's users db.

### When to use?

- Avoid development, infrastructure and/or integration for user workflows.
- Add different levels of entitlement based on type of Pay TV subscriptions.



## Configuration

### Service Configuration
Once the client has aquired a license for Adobe Pass Authentication the following data shall be provided by Adobe:

- Resource ID
- Requestor ID
- Secret key
- Public Key

The aforementioned keys shall be configured in the plugin. The following imsage show the plugin condiguration page, UI cconfigurations are part of it and down below they will be explained.

![SS Plugin Config](https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/Adobe/ss_1.png)

### UI configuration


- **text_color**: Color of the texts present in the screen (excluding button text)
- **code_bg_color**: Color of the square that contains the activation code
- **code_text_color**: Color of the text in the activation code
- **btn_text_color**: Color of the text inside the button
- **bg_color**: Background color of the screen
- **btn_bg_color**: Background color of the button


# Contact Third Party
[Click Here](https://www.toolboxtve.com/solutions/cloud-pass/) to learn more about Toolbox Cloud Pass. 



### Pricing

[Click Here](https://chartbeat.com) to learn more about Toolbox Cloud Pass Pricing. 


**Potential Future Features Include:**

Single Sing On (SSO): The user authenticates once through Cloud Pass in one paticular platform. The user keeps the session open and can access content in other platforms without signing in again. This flow can work only if the other platform(s) has Cloud Pass as a login method.