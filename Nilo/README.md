# Nilo

*Built by LATAM Team*

**Supports:** *iOS and Android*
*Current Version: 0.2.4*

## What is it?

 Nilo is a content aggregator that builds an easy to consume, intuitive and informative timeline of events. Content can be populates statically or in real time, feeding from different sources using several formats such as text, video, images, links and polls. 

## What needs does it meet?


### Design

Render information in a stylish manner. Nilo uses the concept of cards to show all its different formats; each card has an specific context, hence specific functionalities as well.

### One Subject - Many formats

Editorial teams are not bound to show information related to one subject using one restricted format. A sports feed can be composed by articles, images, specific sponsors and polls.

### Living the moment

Users don’t have to go away of your main experience in the app to follow a live event. Nilo allows a reporter or writer covering live events to use any of the cards formats and feed them into a live feed. 

### Engaging Experience and Social Networks

Give the user the tools to interact by sharing content or asking for his input in subjects relevant to him/her.

## When to use?

- The app requieres flexibility in its range of formats to present information.
- The app will serve as conduit for better customer relationship and satisfaction.
- Content generators want to have information ready and available as soon as possible.
- Appealing, easy to use and interactive tools to engage with the user.

## Analytics

- Streaming source change. Each time the player begins the playback of a channel or a live event an event is triggered and it can be send to a specific endpoint.


## Related Technologies

Due to its video nature the live switcher experience can be improved by adding one or both of the following technologies:

**DAI (Dynamic Add Insertion)**. This product popularized by cloud providers such as Google and AWS take the streaming and can replace commercials using digital Que Tones. In this way a network can have a linear commercialization and another for streaming, monetizing both platforms.

**DFP (Doubleclick For Publishers).** This is a well known product to add pre rolls, mid rolls and post rolls to a streaming video. Generally this is better combined with VOD but a live streaming can benefit by adding a pre roll before playback.
\*DFP is part of the plugin and it should only need proper configuration.

## Sources of Content

Nilo can be fed from 3 different types of sources of content:

- Zapp Pipes Feed compatible Data Source Provider.
- Starlight CMS events (http://cms.applicaster.com).
- Social mirrorining from social accounts (Instagram & Twitter).

Any combination of all 3 source types can be combined in a single Nilo screen configuration to display an aggregated timeline of content that shows events from various different sources. A single Nilo screen could display content from CMS, Zapp Pipes Feed, Instagram, and Twitter.

Cards that come from social events will show the social media logo. Cards that come from the Starlight CMS will show the sender thumbnail.

Content events are shown in the form of "Cards", with the following types:

- Video Card: card used to play video.
- Image Card: card used to display an image.
- Article Card: card used to display an article with image/video.
- Link Card: card used to direct the user to an external url.
- Text Card: card used to display a plain text message.


## Configuration

### Live Feed Set Up

Before beginning the configuration, please make sure your account has been set up by support and you have access to the Applicaster CMS.

1.- Go to http://cms.applicaster.com and login.

2.- Once inside enter the name of your account, it should appear as an option you can select.

![image\_1][image-1]

3.- From the menu, select Feed & Interactive.

![image\_2][image-2]

4.- To create the feed click on “New TV Show”.

![image\_2][image-3]


	4.1 Give a clear name so it makes reference to what the context is going to be about.
	
	4.2 Add an image to give identity to the feed (optional).

![image\_2][image-4]

5.- Once created the TV Show, go to “Actions” and select “Enter Feed”

![image\_2][image-5]

6.- The first time entering the TV Show, the creation of a new feed is needed.

![image\_2][image-6]

7.- As the last step before creating Nilo Cards. Create a new episode by clicking “New Episode” in the TV Show dashboard.

![image\_2][image-7]

	7.1.- If the feed is not gonna be temporal set the date to be 1+ year ahead.
	
	7.2.- Upload a logo to have an avatar to be included in the feed cards.


![image\_2][image-8]


8.- The final result will show an upcoming event.

![image\_2][image-9]

### Live Feed Cards

- Once in the TV Show Dashboard an episode should be “Live” to start adding cards to the feed.

![image\_2][image-10]

- Enter the event and click on “New Event”. You have two buttons available to activate the cards menu.

![image\_2][image-11]


#### Text Card

The “Text Card” allows to post a brief paragraph of information. This follow a simple text format with no other elements combined.

	a.- Text. The text to show 
	
	b.- Choose the event source. One feed can mix several events, by selecting one in particular it will brand the card to do reference to it.

![image\_2][image-12]

	c.- Trigger Scheduled. A card can be created and be published at an specific time. A client can benefit from scheduling a series of cards during a live streaming event, marketing campaigns, etc…

![image\_2][image-13]

After creating the card, it will show ready to be publish.

![image\_2][image-14]

The card will look in the app as follows:

	a.- Name of the event the card belongs to.
	b.- Time since publishing.
	c.- Text message.
	d.- Event Avatar.

![image\_2][image-15]

#### Image Card

The “Image Card” allows to post an Image with a brief description text.

	a.- Text. Description of the image. 
	
	b.- Choose the card event source.
	
	c.- Image for the card.
	
	d.- Trigger Scheduled. Program the publishing of the card at an specific time.

  *Consider to use images with 16:9 Apect Ratio. Preferably 1280x720.

![image\_2][image-16]


The card will look in the app as follows:

	a.- Name of the event the card belongs to.
	b.- Time since publishing.
	c.- Brief description.
	d.- Card Image.
	e.- Event Avatar.

![image\_2][image-17]

#### Video Card

The “Video Card” allows to post a Video with a brief description text.

	a.- Text. Description of the Video. 
	
	b.- Choose the card event source.
	
	c.- Image to present while video is loading for playback.
	
	d.- Card Video. The card is aim to play shot format videos. Videos are limited to 1mb 			size.
	
	e.- Trigger Scheduled. Program the publishing of the card at an specific time.

![image\_2][image-18]

The card will look in the app as follows:

	a.- Name of the event the card belongs to.
	b.- Time since publishing.
	c.- Brief description.
	d.- Video Image.
	e.- Event Avatar.
	
	*Video will play in loop while in focus

![image\_2][image-19]

#### Link Event Card

The “Link Event Card” allows to post a Video with a brief description text.

	a.- Text. Brief description of the Link Card. 
	
	b.- Choose the card event source.
	
	c.- Actual URL for the link.

![image\_2][image-20]

	d.- Preview Image. This image will the main part of the card, referencing the link 				context.
	
	e.- Trigger Scheduled. Program the publishing of the card at an specific time.	
	
	*Configurations presented for the webview don’t apply for “Nilo Link Event Cards”.

![image\_2][image-21]

The card will look in the app as follows:

	a.- Name of the event the card belongs to.
	b.- Time since publishing.
	c.- Preview Image.
	d.- Event Avatar.
	e.- Brief text about the link.

![image\_2][image-22]

## DSP Feed

### Link and Link Event Card

To create the card through DSP the json object should have the following base structure:

```
{
      "type": {
        "value": "link"
      },
      "id": "1",
      "title": “applicaster.com”,
      "published": "2019-05-03T13:57:36-05:00",
      "updated": "2019-05-03T13:57:36-05:00",
      "link": {
        "rel": "alternate",
        "type": "html",
        "href": "https://www.applicaster.com"
      },
      "media_group": [
        {
          "type": "image",
          "media_item": [
            {
              "type": "image",
              "key": "image_base",
              "src": “https://www.applicaster.com/hs-fs/hubfs/Retake_and_Own_Your_Audience/eGuide-asset-1.png?width=1030&name=eGuide-asset-1.png"
            }
          ]
        }
      ],
      "author": {
        "name": "Arturo"
      }
    }
```

![image\_2][image-23]

The card will look in the app as follows:

	a.- media group—>content_item—>src
	b.- title

On touch the card will open the link on a full screen web view.

![image\_2][image-24]

### Article Card

To create the card through DSP the json object should have the following base structure:

```
{
      "type": {
        "value": "article"
      },
      "id": "2",
      "category": "APPLICASTER NEWS",
      "title": "Applicaster: grandes expectativas en la región",
      "summary": "Applicaster estuvo en Natpe Miami.",
      "published": "2019-05-03T13:57:36-05:00",
      "updated": "2019-05-03T13:57:36-05:00",
      "link": {
        "rel": "alternate",
        "type": "text/html",
        "href": "http://www.prensario.net/18935-Applicaster-grandes-expectativas-en-la-region.note.aspx"
      },
      "content": {
        "type": "html",
        "content": "<p></p><p>'Es el primer año que llevamos como compañía organizada en Miami, tenemos nuestra propia estructura y actuamos como entidades independientes. Nos podemos enfocar en las necesidades de cada uno de los territorios, tenemos una plataforma que nos permite ser muy competitivos para adaptarnos a las necesidades del cliente', explicó Tapias.</p><p>La empresa tiene nuevos negocios en Miami y Latinoamérica, territorios donde además tiene el apoyo de sus clientes, que se están diversificando hacia más apps dentro de sus productos. ‘Hemos visto una evolución a la proliferación de target dirigido y a marcas más concretas, para desarrollar relación usuario-marca’, destacó.</p><p>El equipo está distribuido entre Miami, España, Nueva York y Colombia, destaca entre sus clientes a Televisa, donde acaba de lanzar el Canal de las Estrellas de Televisa para Android, Apple y Apple TV, también con America TV, y Medcom en Panamá entre otros.</p><p>En el marco de Natpe Miami, Applicaster anunció un acuerdo con TVX de El Salvador y cerró más desarrollos, que Laura Tapias espera poder dar a conocer próximamente.</p><p style='text-align: right;'><strong>Por Emira Sanabria, corresponsal Miami</strong></p><p></p>"
      },
      "media_group": [
        {
          "type": "image",
          "media_item": [
            {
              "type": "image",
              "key": "image_base",
              "src": "http://www.prensario.net/Multimedios/imgs/25758_468.jpg?v=4"
            }
          ]
        }
      ],
      "author": {
        "name": "Notimex"
      },
      "color": "#FF006699",
      "extensions": {
        "color": "#FF006699"
      }
    }


```

![image\_2][image-25]

The card will look in the app as follows:

	a.- media group—>content_item—>src
	b.- category
	c.- title
	d.- summary

![image\_2][image-26]

The article will expand full screen and will show the content—>src value as the article body.

	a.- Close button
	b.- content—>content

![image\_2][image-27]

### Image Card

To create the card through DSP the json object should have the following base structure:

```
{
      "type": {
        "value": "image"
      },
      "id": "3",
      "category": "APPLICASTER MEMORIES",
      "title": "Applicaster at NAB 2018",
      "published": "2019-05-03T13:58:36-05:00",
      "updated": "2019-05-03T13:58:36-05:00",
      "content": {
        "type": "image/jpg",
        "src": "https://pbs.twimg.com/media/Da7DGYNWsAAJqNT.jpg"
      },
      "author": {
        "name": "Arturo"
      }
    }
}

```
![image\_2][image-28]


The card will look in the app as follows:

	a.- content—>src
	b.- title

The cars will expand to fullscreen on touch.

![image\_2][image-29]


### Video Card

To create the card through DSP the json object should have the following base structure:

```
{
      "type": {
        "value": "video"
      },
      "id": "4",
      "category": "APPLICASTER VIDEOS",
      "title": "VIDEO CARD",
      "summary": "TEST",
      "published": "2019-05-07T13:58:36-05:00",
      "updated": "2019-05-07T13:58:36-05:00",
      "content": {
        "type": "video/hls",
        "src": "https://devstreaming-cdn.apple.com/videos/streaming/examples/bipbop_4x3/bipbop_4x3_variant.m3u8"
      },
      "media_group": [
        {
          "type": "image",
          "media_item": [
            {
              "type": "image",
              "key": "image_base",
              "src": "http://www.prensario.net/Multimedios/imgs/25758_468.jpg?v=4"
            }
          ]
        }
      ],
      "author": {
        "name": "Arturo"
      }
```

The card will look in the app as follows:

	a.- content—>src
	b.- title
	c.- summary

![image\_2][image-30]

### Apendix

#### media_item Object

![image\_2][image-31]

## Social

Nilo can use the API for tweeter and Instagram to integrate the client’s social feeds.

Please contact support in order to configure Twitter or Instagram support@applicaster.com

**The following documentation is aimed for Applicaster Support.**

### Configuration

To enable Nilo to use any of the social accounts configured, go to UI Builder and the screen configured with the Episode ID.


![image\_2][image-32]

### Twitter


Open the following URL in a private or incognito window to prevent linking a personal account. Enter the credentials for the account.

https://social-media-aggregator-prod.herokuapp.com/api/twitter-login-redirect?episodeId={episodeID}



Parameters:

- episodeID.

  - To acquire use the following collection in Postman. https://www.getpostman.com/collections/e33ac8480bc37bc15f0c.
    - Dowload postman from [here](https://www.getpostman.com/downloads/).
    - Open postman and add the collection to your workspace.
      1.- You can use the workspace by default or creat a new personal workspace.
      2.- Select collections.
      3.- Click on import.
      ![image\_2][image-38]

    - In the import window select "Import From Link". Enter the link for the collection and click on "Import" button.
      ![image\_2][image-39]


  - Use the method “GET All configurations” to acquire your feed ID or “GET Configuration by ID” if you already have the ID. See the example below.

```
{
        "_id": "5cbe5a191bebd500049d1fcc",
        "episodeTitle": “Episode Test",
        "endTime": 1556237960,
        "startTime": 1556065160,
        "timelineTitle": "Product Test",
        "episodeId": "5cbe5a18f8292f4a9bdfef48",
        "accountId": "5aa98c3bd7c3ef0008754666",
        "timelineId": "5ca7a8d78f6260436de2ecfb",
        "pollingInterval": 30,
        "instagramJobId": -1,
        "facebookJobId": -1,
        "twitterJobId": -1,
        "aggregationJobId": 104257621,
        "starsJobId": 28328914,
        "__v": 0
    }
```

![image\_2][image-33]


As final step use the method “PUT Configuration” go to the Body section and leave “id” and “twitterScreenName” as the only parameters active.

Parameters:

- id. Is the “_id” key available as part of the Configuration response in the previous step.
- twitterScreenName. The username of the twitter account.

  
  1.- Collection Folder.
  2.- Mehotd to use "PUT Configuration"
  3.- Select Body -> form-data  and Check the two parameters aformentioned. Enter both values in reference to the client.  

![image\_2][image-40]

The call should give a response as follows (Twitter account fields should be part of the configuration):

```
{
    "_id": "5cbfb8e20ab2f80004677427",
    "episodeTitle": "Product Episode",
    "endTime": 1614737623,
    "startTime": 1556068723,
    "timelineTitle": "Product Show",
    "episodeId": "5cbfb8e162c47f28b499de2a",
    "accountId": "5aa98c3bd7c3ef0008754666",
    "timelineId": "5cb0c462a491440249a7c973",
    "pollingInterval": 30,
    “instagramJobId": -1,
    "facebookJobId": -1,
    "twitterJobId": 4103993,
    "aggregationJobId": 110728859,
    "starsJobId": 30619780,
    "__v": 0,
    "twitterScreenName": "product2019",
    "twitterAccessTokenKey": "1127986960402923521-vO6Bh8CLJpoQmoVpFbELH8fPd7JFaa",
    "twitterAccessTokenSecret": "jZH5EkYz8M7zCEov919wMj7oxLKyszHFEhbzGNGAopq2H",
    "twitterConsumerKey": "7rhG0ibnaDkpFNw7OPTYbglMr",
    "twitterConsumerSecret": "y9Q8EZ1C5Cs1fun3trIOfd8iSmBjuuwbE05SAPFKdLtxEFt83S",
    "instagramJobId": -1,
        "facebookJobId": -1,
        "twitterJobId": -1,
        "aggregationJobId": 104257621,
        "starsJobId": 28328914,
        "__v": 0
    }
```
### Card Example

![image\_2][image-34]

Instagram

Open the following URL in a private or incognito window to prevent linking a personal account. Enter the credentials for the account.

![image\_2][image-35]


https://social-media-aggregator-prod.herokuapp.com/api/instagram-login-redirect?episodeId={episodeID}

Parameters:

-episodeID. 

	To acquire use the following collection in Postman. https://www.getpostman.com/collections/e33ac8480bc37bc15f0c.
	Use the method “GET All configurations” to acquire your feed ID or “GET Configuration by ID” if you already have the ID. See the example below.

```
{
        "_id": "5cbe5a191bebd500049d1fcc",
        "episodeTitle": “Episode Test",
        "endTime": 1556237960,
        "startTime": 1556065160,
        "timelineTitle": "Product Test",
        "episodeId": "5cbe5a18f8292f4a9bdfef48",
        "accountId": "5aa98c3bd7c3ef0008754666",
        "timelineId": "5ca7a8d78f6260436de2ecfb",
        "pollingInterval": 30,
        "instagramJobId": -1,
        "facebookJobId": -1,
        "twitterJobId": -1,
        "aggregationJobId": 104257621,
        "starsJobId": 28328914,
        "__v": 0
    }
```

To confirm the instagram account has been linked there are two options:

1.- Go to the episode details page.


![image\_2][image-36]


2.- Use the call “Get Configuration” in postman. The response should contain the instagram fields for the account.

```
{
        "_id": "5cbe5a191bebd500049d1fcc",
        "episodeTitle": “Episode Test",
        "endTime": 1556237960,
        "startTime": 1556065160,
        "timelineTitle": "Product Test",
        "episodeId": "5cbe5a18f8292f4a9bdfef48",
        "accountId": "5aa98c3bd7c3ef0008754666",
        "timelineId": "5ca7a8d78f6260436de2ecfb",
        "pollingInterval": 30,
        "instagramAccessToken": "12308291594.0b11f0e.1ed2a241c8f34e029d4394e0d871a3ef",
        "facebookJobId": -1,
        "twitterJobId": -1,
        "aggregationJobId": 104257621,
        "starsJobId": 28328914,
        "__v": 0,
        "instagramUser": {
        "id": "12308291594",
        "username": "appproduct2019",
        "profile_picture": "https://scontent-iad3-1.cdninstagram.com/vp/1db9936ae11fbb38a79a40704859ed2e/5D5480F1/t51.2885-19/44884218_345707102882519_2446069589734326272_n.jpg?_nc_ht=scontent-iad3-1.cdninstagram.com",
        "full_name": "ApplicasterProduct"
    }
}
```   

### Card Example

![image\_2][image-37]

## Detach Social

In order to detach Twitter and/or Instagram from Nilo. Making use of the same Postman Colletion, follow the next steps:

-Gather the ID of your configuration:

  1.- Slect GET All Configurations 
  2.- Hit Send Button
  3.- Click on the response area (where the json apeear) and hit cmd+f for the search bar to appear.
  4.- Use the search bar to find your Episode Name and gather the configuration id.

  ![image\_2][image-41]


- With the configuration ID:

  1.- Select one of the two methods respectively:
    - Instagram: Detach Instagram from Configuration.
    - Twitter: Detach Twitter from Configuration.
  2.- Replace the id configuration in the URL of the method.
  3.- Hit send. The Response will show the details for the account with Instagram of Twitter tokens set to "-1"
 
  ![image\_2][image-42]


[image-1]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_1.png?raw=true
[image-2]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_2.png?raw=true
[image-3]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_3.png?raw=true
[image-4]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_4.png?raw=true
[image-5]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_5.png?raw=true
[image-6]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_6.png?raw=true
[image-7]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_7.png?raw=true
[image-8]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_8.png?raw=true
[image-9]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_9.png?raw=true
[image-10]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_10.png?raw=true
[image-11]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_11.png?raw=true
[image-12]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_12.png?raw=true
[image-13]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_13.png?raw=true
[image-14]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_14.png?raw=true
[image-15]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_15.png?raw=true
[image-16]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_16.png?raw=true
[image-17]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_17.png?raw=true
[image-18]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_18.png?raw=true
[image-19]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_19.png?raw=true
[image-20]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_20.png?raw=true
[image-21]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_21.png?raw=true
[image-22]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_22.png?raw=true
[image-23]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_23.png?raw=true
[image-24]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_24.png?raw=true
[image-25]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_25.png?raw=true
[image-26]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_26.png?raw=true
[image-27]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_27.png?raw=true
[image-28]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_28.png?raw=true
[image-29]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_29.png?raw=true
[image-30]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_30.png?raw=true
[image-31]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_31.png?raw=true
[image-32]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_32.png?raw=true
[image-33]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_33.png?raw=true
[image-34]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_34.png?raw=true
[image-35]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_35.png?raw=true
[image-36]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_36.png?raw=true
[image-37]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_37.png?raw=true
[image-38]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_38.png?raw=true
[image-39]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_39.png?raw=true
[image-40]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_40.png?raw=true
[image-41]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_41.png?raw=true
[image-42]:	https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_42.png?raw=true