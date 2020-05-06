---
layout: post
title: "Bluetooth doesn't support stereo + mic"
date: 2020-05-06
---

At the moment it isn't possible to use Bluetooth 5 (or earlier) with A2DP profile for duplex (playback and capture) 
Bluetooth current implementation doesn't give enough bandwith to have stereo sound and microphone capture at the same time.
Some headsets can support mono sound and mono capture but at a low bitrate. 

Related: [aptX](https://www.aptx.com/products)

Sources:
[superuser.com](https://superuser.com/questions/930251/possible-to-use-bluetooth-headset-in-stereo-mode-with-mic)
```
Your headset needs to support aptX (https://www.aptx.com/products). 
This is a limitation of the bluetooth A2DP profile. Without aptX, it will not 
be able to receive hifi stereo sound one way while sending microphone audio the other way.

And no, contrary to some information floating around in various forums you 
cannot make this work via playing with Windows mixer settings or downloading 
some application. This is why most gaming headsets that do support two-way 
audio in stereo quality don't use bluetooth but a proprietary wireless protocol 
with their own little USB dongle.

EDIT: User "Horn OK Please" below is correct that aptX alone unfortunately 
is no guarantee of this working! You can get aptX headsets that nonetheless 
suffer from the same limitation!
```

```
This is half right. While it's true that gaming headsets use a proprietary protocol, 
just using aptX alone will NOT guarantee that a headset supports duplex (playback and capture) 
audio at high quality (particularly in the playback direction, it'll only be mono channel 
(1 channel) audio and very low bitrate). Only certain models of Creative hardware that 
has to be matched between transceiver and peripheral will work this way. Most aptX 
supporting hardware will not work. – allquixotic Feb 6 '17 at 1:49

@fostandy If you want to use the Bluetooth transceiver inside your laptop, you're 
out of luck, unfortunately. The only Bluetooth transceivers that can work with the 
duplex headsets are USB transceivers, like the Creative BT-W2, which requires 
a compatible Creative-brand Bluetooth headset. So you still need a little dongle 
hanging out of your laptop's USB port. There is no way whatsoever to get 
bidirectional/duplex high-quality stereo audio using the Bluetooth adapter built 
into any laptop, smartphone, desktop, or tablet on the market. 
It's literally 100.0% impossible. – allquixotic Mar 9 '18 at 2:24 
```
