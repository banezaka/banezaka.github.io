---
layout: post
title: "Bluetooth doesn't support stereo + mic"
date: 2020-05-06
---

At the moment it isn't possible to use Bluetooth 5 (or earlier) with A2DP profile for duplex (playback and capture) [superuser source](https://superuser.com/questions/930251/possible-to-use-bluetooth-headset-in-stereo-mode-with-mic)
Bluetooth current implementation doesn't give enough bandwith to have stereo sound and microphone capture at the same time.
Some headsets can support mono sound and mono capture but a at a low bitrate. 

Related topics: [aptX](https://www.aptx.com/products)

```
Your headset needs to support aptX (https://www.aptx.com/products). This is a limitation of the bluetooth A2DP profile. Without aptX, it will not be able to receive hifi stereo sound one way while sending microphone audio the other way.

And no, contrary to some information floating around in various forums you cannot make this work via playing with Windows mixer settings or downloading some application. This is why most gaming headsets that do support two-way audio in stereo quality don't use bluetooth but a proprietary wireless protocol with their own little USB dongle.

EDIT: User "Horn OK Please" below is correct that aptX alone unfortunately is no guarantee of this working! You can get aptX headsets that nonetheless suffer from the same limitation!
```
