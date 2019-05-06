# Video Playlist

*Built by LATAM Team*

**Supports:** *iOS and Android*
*Current Version: 1.1.5*

 
## About

The Video Playlist is a full screen plugin designed to improve the experience between playing through a set of videos within a common context. 

## What needs does it meet?
### Playlist

List of videos with an inline player (At the top of the list). These playlist has several functions:

- Metadata. Each video shown as part of the list can display 3 fields to better described itself:
  - Publish date. Day and hour when the video content was produced.
  - Title. Title better describing the content.
  - Thumbnail. An editorial cover or frame directly from the video.
- Autoplay. Once the list is load, the first video will autoplay in the inline player. The user will start enjoying the content while having the option to traverse the list of videos in the same context.
- Fullscreen. At any moment the user can choose to go fullscreen and focused on the current content playing without distractions.
- Airplay/Chromecast. If the user likes the concept of second screen. He can send the playback directly to the “Big Screen” and continue the playback. The autoplay shall work as expected while using this function. 

### Back to Back Playback

To give a better experience to the user and engage in more content. This function will autoplay the next video on the list right after finishing the current video.


### When to use?

- The client content is well segmented and a video playlist will help engage the user to consume as much content as possible. 
- Promote content in an organic way. Gather content by an editorial team and promote content in a smart way.

## Analytics

- TBD

## Related Technologies

Due to its video nature the live switcher experience can be improved by adding one or both of the following technologies:

**DFP (Doubleclick For Publishers)**. This is a well known product to add pre rolls, mid rolls and post rolls to a streaming video. Generally this is better combined with VOD but a live streaming can benefit by adding a pre roll before playback.

## Configuration

### Feed Structure

Here you can find in detail manner the fields and data necessary to build the specific structure. Keep in mind this structure will define an EPG for single or multiple live channels or live events.

![table_1](https://github.com/applicaster/latam-product-documentation/blob/master/Video_playlist/ss_1.png?raw=true)

### Entry Object

![table_2](https://github.com/applicaster/latam-product-documentation/blob/master/Video_playlist/ss_2.png?raw=true)

### media_item Object

![table_3](https://github.com/applicaster/latam-product-documentation/blob/master/Video_playlist/ss_3.png?raw=true)

### Feed Example

```
    "type": {
        "value": "feed"
    },
    "title": "Últimos Videos",
    "entry": [
        {
            "type": {
                "value": "video"
            },
            "id": "1_oo0p8nzn",
            "category": “Destacado”,
            "title": "Incrementan exponencialmente las desapariciones en Baja California Sur",
            "summary": "El tema de las desapariciones en el estado se ha salido de control, al grado de, como en cualquier otro evento, las autoridades del estado han pedido a la gente que acudan a parques para llevar a cabo tomas de sangre a familiares de desaparecidos.",
            "published": "2019-03-27T23:30:00-06:00",
            "updated": "2019-03-27T23:30:00-06:00",
            "link": {
                "rel": "alternate",
                "type": "text/html",
                "href": "http://myapi.com.mx/incrementan-exponencialmente-las-desapariciones-en-baja-california-sur/2500890"
            },
            "content": {
                "type": "video/hls",
                "src": “http://mydnc.ne/mycontent.m3u8”
            },
            "content_group": [
                {
                    "type": "image",
                    "content_item": [
                        {
                            "type": “image",
                            "key": "image_base",
                            "src": “http://mycdn.net/myimage.png“
                        }
                    ]
                }
            ],
        },
```

### UI Builder configuration

Please follow the next steps to add VideoPlaylist to your application.

**1.-** Once the data feed(described in this document) is available, go to the Feed section, with JSON Feed data type.

![image_1](https://github.com/applicaster/latam-product-documentation/blob/master/Video_playlist/ss_4.png?raw=true)

**2.-** Go to the Plugins and search for VideoPlaylist. Add it to your layouts.

![image_2](https://github.com/applicaster/latam-product-documentation/blob/master/Video_playlist/ss_5.png?raw=true)

**3.-** Go to layouts in the main side menu. Select Add Screen from the bottom of the layouts list, search for Video Playlist and add it to your current screen.

**4.-** Select the Video Playlist layout and follow the instructions below.

#### Data Section
- Select Json Feed as Type.
- As Source select the feed you created previously.
#### General Section
- Select Video Playlist as Content Type.

![image_3](https://github.com/applicaster/latam-product-documentation/blob/master/Video_playlist/ss_6.png?raw=true)

### Notes

**Known issues** 

The plugin will not respond to the properties under the STYLES section. If customization for styles is needed a developer must hard code the changes.
