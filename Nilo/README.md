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
*DFP is part of the plugin and it should only need proper configuration.

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

###Live Feed Set Up

Before beginning the configuration, please make sure your account has been set up by support and you have access to the Applicaster CMS.

1.- Go to http://cms.applicaster.com and login.

2.- Once inside enter the name of your account, it should appear as an option you can select.

![image_1](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_1.png?raw=true)

3.- From the menu, select Feed & Interactive.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_2.png?raw=true)

4.- To create the feed click on “New TV Show”.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_3.png?raw=true)


    4.1 Give a clear name so it makes reference to what the context is going to be about.

    4.2 Add an image to give identity to the feed (optional).

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_4.png?raw=true)

5.- Once created the TV Show, go to “Actions” and select “Enter Feed”

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_5.png?raw=true)

6.- The first time entering the TV Show, the creation of a new feed is needed.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_6.png?raw=true)

7.- As the last step before creating Nilo Cards. Create a new episode by clicking “New Episode” in the TV Show dashboard.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_7.png?raw=true)

    7.1.- If the feed is not gonna be temporal set the date to be 1+ year ahead.

    7.2.- Upload a logo to have an avatar to be included in the feed cards.


![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_8.png?raw=true)


8.- The final result will show an upcoming event.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_9.png?raw=true)

### Live Feed Cards

- Once in the TV Show Dashboard an episode should be “Live” to start adding cards to the feed.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_10.png?raw=true)

- Enter the event and click on “New Event”. You have two buttons available to activate the cards menu.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_11.png?raw=true)


#### Text Card

The “Text Card” allows to post a brief paragraph of information. This follow a simple text format with no other elements combined.

    a.- Text. The text to show 

    b.- Choose the event source. One feed can mix several events, by selecting one in particular it will brand the card to do reference to it.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_12.png?raw=true)

    c.- Trigger Scheduled. A card can be created and be published at an specific time. A client can benefit from scheduling a series of cards during a live streaming event, marketing campaigns, etc…

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_13.png?raw=true)

After creating the card, it will show ready to be publish.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Nilo/ss_14.png?raw=true)

The card will look in the app as follows:

	a.- Name of the event the card belongs to.
	b.- Time since publishing.
	c.- Text message.
	d.- Event Avatar.












#### Image Card

The “Image Card” allows to post an Image with a brief description text.

	a.- Text. Description of the image. 
	
	b.- Choose the card event source.
	
	c.- Image for the card.
	
	d.- Trigger Scheduled. Program the publishing of the card at an specific time.















The card will look in the app as follows:

	a.- Name of the event the card belongs to.
	b.- Time since publishing.
	c.- Brief description.
	d.- Card Image.
	e.- Event Avatar.

#### Video Card

The “Video Card” allows to post a Video with a brief description text.

	a.- Text. Description of the Video. 
	
	b.- Choose the card event source.
	
	c.- Image to present while video is loading for playback.
	
	d.- Card Video. The card is aim to play shot format videos. Videos are limited to 1mb 			size.
	
	e.- Trigger Scheduled. Program the publishing of the card at an specific time.






The card will look in the app as follows:

	a.- Name of the event the card belongs to.
	b.- Time since publishing.
	c.- Brief description.
	d.- Video Image.
	e.- Event Avatar.

	*Video will play in loop while in focus









#### Link Event Card

The “Link Event Card” allows to post a Video with a brief description text.

	a.- Text. Brief description of the Link Card. 
	
	b.- Choose the card event source.
	
	c.- Actual URL for the link.

	d.- Preview Image. This image will the main part of the card, referencing the link 				context.

	e.- Trigger Scheduled. Program the publishing of the card at an specific time.	
	
	*Configurations presented for the webview don’t apply for “Nilo Link Event Cards”.







The card will look in the app as follows:

	a.- Name of the event the card belongs to.
	b.- Time since publishing.
	c.- Preview Image.
	d.- Event Avatar.
	e.- Brief text about the link.

#### Social 

Twitter and Instagram social mirroring must be configured in the Starlight CMS timeline that corresponds to the timelineId indicated.

Please contact support in order to configure Twitter or Instagram support@applicaster.com
























