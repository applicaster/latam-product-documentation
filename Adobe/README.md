
# Adobe Primetime Authentication 

*Built by LATAM Team*

**Supports:** *iOS, Android, Android TV, tvOS, FireTV and Roku*

**Current Versions:**
- *5.0.3 (iOS)*
- *0.1.5 (Android)*
- *5.0.3 (tvOS)*
- *0.1.5 (Android TV)*
- *5.0.3 (FireTV)*
- *1.0.0 (Roku)*
 
## About
Cloud Pass is designed to authenticate and authorize users serving as the interconnection between content providers and TV Operators.



### What needs does it meet?

- Handles the auhentication and authorization through TV Operators users DB.
- Different levels of authorizarization through the user subscription


### When to use?

- Want to show your content but restricti playback to TV Operators subscription
- There are different levels of premium content


## Configuration

1.- Toolbox shall provide an apiKey. This apiKey is exclusive for you and is not shared amongst content providers.
2.- The following paramteres are part of the plugin configuration and will help to have succesfull UI/UX and behavior:

### Android:
  - **shortname (String)**: Content provider shortname (i.e NBC, CBS, PBS, etc...).
  - **apiKey (Hash)**: Unique toolbox apiKey to consume Cloudpass Services.
  - **company_logo_url (URL)**: Logo to display on the header of the cable operator screen.
  - **cable_operator_selection_header_text (String)**: Quick text to give context of this login access.
  - **login_navbar_background_color (HEX Color)**: Login screen top navigation background color.
  - **login_navbar_title_color (HEX Color)**: Login screen top navigation title color.
  - **login_navbar_title (String)**: Commonly one or two words giving context in the main top nav bar of the app.
  - **logout_dialog_title (String)**: Title of the logout dialog. The plugin considers the logout action as well.
  - **logout_dialog_message (String)**: Message to ask the user and make him/her aware of the action about to take place.
  - **logout_dialog_positive_button_text (String)**: Text for the button to accept and log out.
  - **logout_dialog_negative_button_text (String)**: Text for the button to cancel the log out action.

![SS Plugin Config](https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/toolbox-cloud-pass/ss_1.png)


### iOS:
  - **shortname (String)**: Content provider shortname (i.e NBC, CBS, PBS, etc...).
  - **apiKey (Hash)**: Unique toolbox apiKey to consume Cloudpass Services.
  - **company_logo_url (URL)**: Logo to display on the header of the cable operator screen.
  - **cable_operator_selection_header_text (String)**: Quick text to give context of this login access.

![SS Plugin Config](https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/toolbox-cloud-pass/ss_2.png)




# Contact Third Party
[Click Here](https://www.toolboxtve.com/solutions/cloud-pass/) to learn more about Toolbox Cloud Pass. 



### Pricing

[Click Here](https://chartbeat.com) to learn more about Toolbox Cloud Pass Pricing. 
