# Live Switcher

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
 **type** | "An object containing a value. This used to give meaning to this section. | **Object**
 ||-**value** : A **string** that references the use for this Json response. For this context “feed” shall be the value." ||
 **title** |	A string to describe the feed.	| **String**
 **entry**|	List of entry Object defining the program schedule for an specific channel or live event.	|**Object**
 **extensions**	|An object to specify custom key/value pairs or json objects. Refer to extensions Object.	|**Object**

### Entry Object

Parameter | Description | Type
---------|----------|---------
 **type** | "An object containing a value. This used to give meaning to this section. | **Object**
 ||- **value** : A **string** that references the use for this json response. For this context “**program**” shall be the value.|
 **id** | A numeric incremental value to identify the entry object. | **Integer**
 **author** | Does not apply for this particular context | **String**
 **summary** | A string with a brief description of the program. | **String**
 **media_group** | An object that can contain different types of media item objects.| **Object**
 ||- **type** : Indicates how the media_item object should be treated. For this context “image” shall be used. This image will graphically reference the video content.|
 ||- **media_item** : refer to media_item Object.|
 **content** | An object that can be used to defined the media referenced by the entry.| **Object**
 ||- **type** : Indicates the type of media content is referenced by the entry. For this context **“video/hls”** shall be used.||
 ||- **src** : A **url string** referencing the media asset source.|
 **extensions** | An object to specify custom key/value pairs or json objects. For this context the following key/value pairs shall be considered:|**Object**
 ||- **start_time** : timestamp indicting the beginning of the timeframe cover by the specific entry. Format *YYYY-MM-DDThh:mm:ss—hhmm*.||
 ||- **end_time** : timestamp indicting the beginning of the timeframe cover by the specific entry. Format *YYYY-MM-DDThh:mm:ss—hhmm*.|| 
 ||- **applicaster_channel_id** : A incremental integer referencing the live channel configured in Applicaster 2." ||

 ### Media_item Object

Parameter | Description | Type
---------|----------|---------
 **src** | A **url string** referencing to the media asset source. | **String**
 **key** | A **string** to identify among other the media_item objects.  | **String**
 **type** | A **string** to define the kind of media asset. | **Object**


### Extensions Object

Parameter | Description | Type
---------|----------|---------
 **channels** | "A custom  **array** field containing channel objects for this particular context.|**Array**
 ||- **Channel Object**: An object containing specific data for each live channel. Refer to channel Object. | 

 ### Channel Object
Parameter | Description | Type
---------|----------|---------
 **name** | A  **string** to define the name of a specific channel. | **Array**
 **id** | A incremental  **integer** referencing to which Applicaster channel the data belongs to. | **Array**
 **logo** | A  **string** url referencing the media asset source. This image will be displayed as the logo for the specific channel. | **Array**

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

![Semantic description of image](https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/Live-Switcher/ss_1.png)

2.- Go to the Plugins and search for LiveChannelsReactNative. Add it to your layouts.

![Semantic description of image](https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/Live-Switcher/ss_2.png)

3.- Go to layouts in the main side menu. Select Add Screen from the bottom of the layouts list, search for Video Playlist and add it to your current screen.

![Semantic description of image](https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/Live-Switcher/ss_3.png)

4.- Select the Video Playlist layout and follow the instructions below.

![Semantic description of image](https://raw.githubusercontent.com/applicaster/latam-product-documentation/master/Live-Switcher/ss_4.png)

##### Data Section
-Select Json Feed as Type.
-As Source select the feed you created previously.
##### General Section
-Select Channel Switcher as Content Type.

## Notes

#### **Single Channel EPG**

Each channel will show an icon to display the entire schedule available. This should follow the normal process to configure an EPG in Applicaster 2. Please Refer to the specific documentation.

#### **Known issues** 

The plugin will not respond to the properties under the STYLES section. If customization for styles is needed a developer must hard code the changes.