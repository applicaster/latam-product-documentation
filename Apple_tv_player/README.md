## Apple TV Player

### What is it?

Video Player based on AVPlayer libraries.

## What needs does it meet?


### Subtitles and Audio

If available as part of the HLS protocol, subtitles and audio will be shown as options.

### Ads

Advertisement through DFP has been fixed.

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

- Add the “Olympic Channel Player” plugin to the app.

- The player will act as the default player.

- The following fields define the player behavior:



1.- Add the ID for the Youbora account to which the events and data will be reported back.

![image_1](https://github.com/applicaster/latam-product-documentation/blob/master/Apple_tv_player/ss_1.png?raw=true)

UI/UX

It makes use of the default UI/UX on tvOS.