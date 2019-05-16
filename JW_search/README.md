
# JW Search

*Built by LATAM Team*

**Supports:** *iOS and Android*
*Current Version iOS: 0.0.10*
*Current Version Android: 0.1.3*

 
## About
JW Platform offers a basic search component. Any client using JW Platform as their CMS for video can benefit of a basic search in their app.

### What needs does it meet?

- Search engine wihtout any added infrastructure cost.
- Limit of itmes and pagination
- Metadata


### When to use?

- The client has JW PLatform as CMS
- The amount of content overpasses the ability to be discovered in fullness through the sections and views in the app.


## Configuration

The configuration is devided between JW PLatform Dashboard and UI Builder.

### JW Platform Dashnoard

- Once inside the dashboard select **Playlists** from the videos menu.

![image\_2][image-1]

- Click on **Create** button and select **Search** as the type of playlist to create.

![image\_2][image-2]

![image\_2][image-3]

- Inside the playlist details page there are several settings to personalise the bevavior.USe the **SETUP** subsection .

    1.- Filter by Tag - Include videos with. Restrain the search to only respond with videos containing specific tags and the text being searched.
    2.- Filter by Tag - Exclude videos with. Exclude videos with specifics tags to be returned in the search response.
    3.- Promoted content. Not applicable at this moment to the product.
    4.- List Lenght. Maximum records to be returned by the search. This value can be paginated to improve the experience and time of response by the search. 

![image\_2][image-4]

- Use the **Developer Resources** section to obtain the URL for JSON and RSS formats. This URL will be set up as part of the plugin.
    - The parameter **search** will be the input value for the search.

![image\_2][image-5]

### UI Builder

- Once inside UI Builder go to **plugins->My PLugins** . Find the **JW Search Plugin** and install it.

![image\_2][image-6]
  
- The plugin will be available as a screen. This allow it to be actioned by any component.

- There are two settings to configure to make the plugin functional:
  - Base URL. The URL gathered through the JW Platform which references the search playlist
  - Page Limit. Amount of itmes to be requested. The pagination will load more items at the same rate each time the last item is reached while scrolling the list.

Visual example of the search.



## Logging Events

TBD


# Contact Third Party
[Click Here](https://www.jwplayer.com/) to learn more about Cheartbeat. 



### Pricing

Contact JW Player for more information.








[image-1]:	https://github.com/applicaster/latam-product-documentation/blob/master/JW_search/ss_1.png?raw=true
[image-2]:	https://github.com/applicaster/latam-product-documentation/blob/master/JW_search/ss_2.png?raw=true
[image-3]:	https://github.com/applicaster/latam-product-documentation/blob/master/JW_search/ss_3.png?raw=true
[image-4]:	https://github.com/applicaster/latam-product-documentation/blob/master/JW_search/ss_4.png?raw=true
[image-5]:	https://github.com/applicaster/latam-product-documentation/blob/master/JW_search/ss_5.png?raw=true
[image-6]:	https://github.com/applicaster/latam-product-documentation/blob/master/JW_search/ss_6.png?raw=true
[image-7]:	https://github.com/applicaster/latam-product-documentation/blob/master/JW_search/ss_7.png?raw=true
[image-8]:	https://github.com/applicaster/latam-product-documentation/blob/master/JW_search/ss_8.png?raw=true
[image-9]:	https://github.com/applicaster/latam-product-documentation/blob/master/JW_search/ss_9.png?raw=true