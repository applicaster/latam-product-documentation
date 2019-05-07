# Android TV Player

*Built by LATAM Team*

**Supports:** *Android*
*Current Version: 1.1.5*

## What is it?

Video Player based on EXO Player libraries.

## What needs does it meet?

### Platforms

The player is functional in both Android Mobile and Android TV.

### Design

Improved from what the basic Android Player has out of the box. Controls can be improved and the whole UI Overall yet it looks clean and simple.

### Subtitles and Audio

If available as part of the HLS protocol, subtitles and audio will be shown as options.

### Ads

Advertisement through DFP has been added. Skip functionality is available as well.

### Automatic Language and Subtitles

The player will identify the language of the device and automatically select the audio track or subtitles if available.

## When to use?

- Better integration with HLS Protocol overall.
- Advertisement needed.

## Analytics

**Youbora** is the platform supported out of the box.

All standard events are tracked:

- media resource
- throughput
- bitrate
- rendition

Additionally two of the three extra items available are reported back:

- title
- isLive

## Configuration

- Add the “Android TV Player” plugin to the app.

- The player will act as the default player.

- The following fields define the player behavior:

1.- Add the ID for the Youbora account to which the events and data will be reported back.

2.- Will disable Audio and Subtitles options from the player. Icon will be hidden and there will not be access to the options view.

3.- Enable debug mode to get specific video settings and parameters for the asset played by the player.

4.- “AndroidTV” or “FireTV” are the values accepted. This parameter is important for reporting correctly with platform is generating analytics.

## UI/UX

### Controls
1.- Play/Pause Button. The button will dynamically change its function and icon according to the state of the video.

2.- Time elapsed.

3.- Time remaining.

4.- Audio and Subtitles Button. The button will hide the video controls and show the list of audios and subtitles available for the current video in another overlay view.

5.- Title. It shows the title of the current video. This is taken directly from the metadata available.


## Audio and Subtitles View

1.- Audio tracks available.

2.- Subtitles available.
