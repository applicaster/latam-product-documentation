# Live Switcher

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

## What is it?

The live switcher is a full screen plugin designed for video streaming purposes. It displays a set of channels or live events related to a specific context.

## What needs does it meet?
### Live Channels
By itself the live switcher can show the whole lineup of live channels available to the user. By having an inline player at the top of the list, a user can easily switch between streamings without going in and out of fullscreen video.

### Single Channel EPG
Where live channels are present, an EPG is needed. The live switcher can add the functionality to have an EPG per channel. In this way a the content of a channel can be clearly communicated to the user and engage him.

### Live Events
The list of channels can be used in conjunction to display live events or as a solely live events list. Each event has its schedule and also a friendly reminder can be set.

### When to use?

- Several channels need to be displayed and make the user aware of the offer.
- Simulate the familiarity a user has with the easy switch between channels in a TV.
- Promote live events as part of the streaming offer. 
- A better experience  making a combination of different elements (Video Player, reminders and EPG)

## Analytics

- Streaming source change. Each time the player begins the playback of a channel or a live event an event is triggered and it can be send to a specific endpoint.

## Related Technologies

Due to its video nature the live switcher experience can be improved by adding one or both of the following technologies:

**DAI (Dynamic Add Insertion)**. This product popularized by cloud providers such as Google and AWS take the streaming and can replace commercials using digital Que Tones. In this way a network can have a linear commercialization and another for streaming, monetizing both platforms.

**DFP (Doubleclick For Publishers)**. This is a well known product to add pre rolls, mid rolls and post rolls to a streaming video. Generally this is better combined with VOD but a live streaming can benefit by adding a pre roll before playback.

## Configuration

### Feed Structure

Here you can find in detail manner the fields and data necessary to build the specific structure. Keep in mind this structure will define an EPG for single or multiple live channels or live events.



Parameter | Description | Type
---------|----------|---------
 <span style="color:red"> type </span> | "An object containing a value. This used to give meaning to this section. <br/><br/>- **value** : A <span style="color:red">string</span> that references the use for this Json response. For this context “feed” shall be the value." | <span style="color:blue"> Object </span>
 <span style="color:red">title</span> |	A string to describe the feed.	| <span style="color:blue"> String </span>
 <span style="color:red">entry</span>|	List of entry Object defining the program schedule for an specific channel or live event.	|<span style="color:blue"> Object </span>
 <span style="color:red">extensions</span>	|An object to specify custom key/value pairs or json objects. Refer to extensions Object.	|<span style="color:blue"> Object </span>

### Entry Object

Parameter | Description | Type
---------|----------|---------
 <span style="color:red">type</span> | "An object containing a value. This used to give meaning to this section.<br/><br/>- **value** : A <span style="color:red">string</span> that references the use for this json response. For this context “**program**” shall be the value.| <span style="color:blue">Object</span>
 <span style="color:red">id</span> | A numeric incremental value to identify the entry object. | <span style="color:blue">Integer</span>
 <span style="color:red">author</span> | Does not apply for this particular context | <span style="color:blue">String</span>
 <span style="color:red">summary</span> | A string with a brief description of the program. | <span style="color:blue">String</span>
 <span style="color:red">media_group</span> | "An object that can contain different types of media item objects.<br/><br/>- **type** : Indicates how the media_item object should be treated. For this context “image” shall be used. This image will graphically reference the video content.<br/>- **media_item** : refer to media_item Object.| <span style="color:blue">Object</span>
 <span style="color:red">content</span> | "An object that can be used to defined the media referenced by the entry.<br/><br/>- **type** : Indicates the type of media content is referenced by the entry. For this context **“video/hls”** shall be used.<br/>- **src** : A <span style="color:red">url string</span> referencing the media asset source.| <span style="color:blue">Object</span>
 <span style="color:red">extensions</span> | "An object to specify custom key/value pairs or json objects. For this context the following key/value pairs shall be considered:<br/><br/>- **start_time** : timestamp indicting the beginning of the timeframe cover by the specific entry. Format <span style="color:green">*YYYY-MM-DDThh:mm:ss—hhmm*</span>.<br/><br/>- **end_time** : timestamp indicting the beginning of the timeframe cover by the specific entry. Format <span style="color:green">*YYYY-MM-DDThh:mm:ss—hhmm*</span>.<br/><br/>- **applicaster_channel_id** : A incremental integer referencing the live channel configured in Applicaster 2." | <span style="color:blue">Object</span>

 ### Media_item Object

Parameter | Description | Type
---------|----------|---------
 <span style="color:red">src</span> | A <span style="color:red">url string</span> referencing to the media asset source. | <span style="color:blue">String</span>
 <span style="color:red">key</span> | A <span style="color:red">string</span> to identify among other the media_item objects.  | <span style="color:blue">String</span>
 <span style="color:red">type</span> | A <span style="color:red">string</span> to define the kind of media asset. | <span style="color:blue">Object</span>


### Extensions Object

Parameter | Description | Type
---------|----------|---------
 <span style="color:red">channels</span> | "A custom  <span style="color:red">array</span> field containing channel objects for this particular context.<br/><br/>- **Channel Object**: An object containing specific data for each live channel. Refer to channel Object. | <span style="color:blue">Array</span>

 ### Channel Object
Parameter | Description | Type
---------|----------|---------
 <span style="color:red">name</span> | A  <span style="color:red">string</span> to define the name of a specific channel. | <span style="color:blue">Array</span>
 <span style="color:red">id</span> | A incremental  <span style="color:red">integer</span> referencing to which Applicaster channel the data belongs to. | <span style="color:blue">Array</span>
 <span style="color:red">logo</span> | A  <span style="color:red">string</span> url referencing the media asset source. This image will be displayed as the logo for the specific channel. | <span style="color:blue">Array</span>

## Feed Example
```
    "type": {
        "value": "feed"
    },
    "title": "Feed EPG",
    "entry": [
        {
            "type": {
                "value": "program"
            },
            "id": "110621",
            "title": "THE VOID",
            "author": {
                "name": ""
            },
            "summary": "An officer is sent to investigate multiple crimes related to a local gang",
            "media_group": [
                {
                    "type": "image",
                    "media_item": [
                        {
                            "src": "http://www.myassets.com/images/thevoidposter.jpg",
                            "key": "image_base",
                            "type": "image"
                        }
                    ]
                }
            ],
            "content": {
                "type": "video/hls",
                "src": "https://mycdn-live.net/live/the_void.m3u8"
            },
            "extensions": {
                "start_time": "2019-02-13T16:00:00-0600",
                "end_time": "2019-02-13T18:00:00-0600",
                "isLive": "true",
                "applicaster_channel_id": "1040"
            }
        },
      ],
      "extensions": {
          "channels": [
              {
                  "name": “My Live Channel",
                  "id": "1038",
                  "logo": “https://mycdn-live.net/logos/mylivechannel.png”
              }
          ]
      }
  }
```

# UI Builder Configuration

Please follow the next steps to add Live Switcher to your application.

1.- Once the data feed(described in this document) is available, go to the Feed section, with JSON Feed data type.

![Semantic description of image](https://drive.google.com/uc?id=1fWMq7vqSxLNrNAtFWNXKImbIcPbzezjo)

2.- Go to the Plugins and search for LiveChannelsReactNative. Add it to your layouts.

![Semantic description of image](https://drive.google.com/uc?id=1WrJZ4SOHOR-t1jVMeQ4vr6zATwnRG6pQ)

3.- Go to layouts in the main side menu. Select Add Screen from the bottom of the layouts list, search for Video Playlist and add it to your current screen.

![Semantic description of image](https://drive.google.com/uc?id=1j_-wRBgIO5vq7iHtny0OCqjTxYC3rmmu)

4.- Select the Video Playlist layout and follow the instructions below.

![Semantic description of image](https://drive.google.com/uc?id=16qinFB5rDyEzoN5u_WeEPijjPPP-z_g3)

##### Data Section
-Select Json Feed as Type.
-As Source select the feed you created previously.
##### General Section
-Select Channel Switcher as Content Type.

## Notes

####<span style="color:#014D7F">Single Channel EPG</span>

Each channel will show an icon to display the entire schedule available. This should follow the normal process to configure an EPG in Applicaster 2. Please Refer to the specific documentation.

####<span style="color:#014D7F">Known issues</span> 

The plugin will not respond to the properties under the STYLES section. If customization for styles is needed a developer must hard code the changes.