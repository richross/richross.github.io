---
layout: posts
title: Audio Configuration
author: Rich Ross
excerpt_separator: <!--more-->
---

This is a long overdue post.  It is a reference post for audio setup for virtual meetings and podcast/videos.  

The story really starts back in 2020 at the start the pandemic when almost everyone was forced to work from home.  As part of that quick effort, I went from in-person meetings to virtual sessions over Teams with customers.  This was a huge shift for everyone involved.  I had a good amount of experience with conducting virtual sessions from broadcasting a weekly show with some friends on twitch and YouTube.  The important component in moving to this medium is not video, but providing high-quality audio.  How you sound goes a long way toward keeping the participants engaged in the discussion.
<!--more-->
I found the high-quality audio setup I used at home was greatly appreciated by those on the call.  I was often asked about what I used and put a 'wishlist' together that I could easily share.  There were also some items I was not able to put on the list and comments to keep in mind when configuring everything.  To help organize the items, this really breaks down into hardware and software.

### Hardware ###
The full list can be found [here](https://www.amazon.com/hz/wishlist/ls/3DJ156DLHHS76?ref_=wl_share).

**Microphone**: Audio Technical AT2020 - I chose this I knew many who had this as their primary mic.  As I started using it, I noticed that it could capture my audio with getting all of the sounds in the room as I had with my previous mic.  For the cost and quality, I think it gives everything you need without having to spend hundreds of dollars on the mic alone.  
Is this the best mic out there today?  Probably not, but it is a great entry level mic, I'm really happy with the setup and not ready to upgrade this part.  

**Boom stand**: One thing I always tell people when it comes to this setup, you have to have the mic right in your face to get the best quality.  Position is also important for visibility.  Being able to see the keyboard when typing.  Being able to be seen if using a camera.  A boom stand lets you find a position where the mic meets all of these criteria.  I included what I use on the list but also like the models from Blue and Elgato so pick what you like.

**Audio Interface**: For the most part, the microphone signal needs to get to some computer.  The computer has USB connections so we need a way to convert from XLR, or pro audio, connector to USB.  I started with a Xenyx mixing board that provided a USB connection, which I plugged into my computer.  My computer is able to see this as an audio source and I can then assign it as my mic for input and my headphones for output.  
I've since switched to a Focusrite Scarlet 2i2 as it is smaller, gets power from the USB connection and let's me mount it under my desk.  As an aside, I'm learning to platy the bass and I like that I can plug my bass into the other input to combine the signal with audio from Spotify while practicing.

### Software ###
Once the audio signal hits the computer, configure the settings in Teams or Skype to use this mic input as the 'microphone'.  Configure the 'speakers' to use where you want to send the audio, which can be either of the audio interfaces defined above or any other audio connected to your computer.

**Virtual Audio Interface**: Not sure if that is the right term, but it is how I think of these applications.  This is software that allows you to define how audio signal is routed between both physcial hardware and virtual / software on your machine.  My favorite for this purpose is [VoiceMeeter Banana](https://vb-audio.com/Voicemeeter/banana.htm).  Banana allows me to take any audio signal on my PC and route it to an appropriate output.  I can take the audio from the Teams call and send it to my speakers, while at the same time send the audio from my music player to my headphones, and then send my mic audio, the Teams audio to my live streaming application.  I'm not going to describe how all of these configurations can be done as there are plenty of tutorials and videos that go through this.  In general, if you can visual everything as the old audio racks of components we had growing up (if you are around my age) it becomes possible to see that everything connects via a virtual cable with an input connecting to an output.  That's what works for me. :)

With all the complexities that Banana has when it comes to signal routing, the thing they make easy and why I keep coming back to installing it on my machine is the 'Intellipan' control.  I'm not an audio engineer.  I can play with the various capabilities and wind up defaulting to the original settings.  That is why 'Intellipan' control is so amazing.  I just move the 'joystick' control to the lower left corner and I get this amazing adjustment to my voice quality that has become a bit of a signature for me.  

I tried using another software for this capability, Elgato's [WaveLink](https://elgato.com), which works with my system given that I am using the new [StreamDeck+](https://www.elgato.com/en/stream-deck-plus).  This was also why I temporarily switched to WaveLink and use the dials to control my audio levels.  There were a couple of downsides for me and my setup.  First, there is no mono button on the WaveLink.  The Focusrite sends the mic in 1 channel so it is only heard in the left or right side.  Banana has a mono button so the signal is sent to both speakers.  This meant to use WaveLink, I had to bring back the Xenyx.  Second complexity is that WaveLink has a plug-in model for the audio configuration.  There is no easy button, like the 'Intellipan' on the Banana.  Plus a simple plug-in often needed another application to host the plug-in on my computer.  While I tried to configure them, I had one of my colleagues asked what happened to my audio configuration as that mellow radio voice was no longer there.

Fortunately, a plug-in was created for the StreamDeck + to allow for changing audio levels with the dials.  So I just swapped everything back to Banana/Focusrite configuration and I'm much happier.  I sound better too. :)

I think this setup will continue to evolve.  I'm reworking my office space at home.  Right now all of my existing audio gear is in the office as we continue to conduct virtual sessions from the office.  I may want to use this as a chance to look at what is out there and improve on the setup.  

Let me know what you are using and if any of this is helpful to your setup.