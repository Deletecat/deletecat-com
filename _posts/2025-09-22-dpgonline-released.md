---
title: dpgonline released!
description: A new, free DPG converter on the web.
---
Moonshell is a cool piece of homebrew for the Nintendo DS.
It supports playing music and videos, displaying images and text files, editing text files, recording audio clips through the microphone, SD card speed testing, alarms... it can do so many different things!

I think it's great, but there's one issue. It only supports video playback with it's own "DPG" format. The DPG format is comprised of MPEG-1 video and MPEG-2 audio, as well as a non-standard group of pictures structure (DPG2+) and a video thumbnail (DPG4). Other audio formats were supported in Moonshell 1.7.1, but that support seems to have been removed with Moonshell 2.

There are many different programs that can be used to convert your media. Moonshell comes bundled with one, it's not great but it will work. The main issue though is that none of them are really focused on mobile or web app support. I've been able to get [dpgv4](https://github.com/pawel-slowik/dpgv4) (my beloved <3) working well on my Android device, but trying to guide others through the steps needed to get it working is not fun.

There are online web converters out there that may work... but all of them that I tried did not give me an output that would work in Moonshell. The closest I found was from a site called "online-convert.com" who seem to have a rough idea of how the format is supposed to be laid out. But the output file unfortunately displays an error when you try to play it back.

There used to be a few sites online that would work going by 16 year old GBATemp posts. You may be shocked to hear that they are no longer around. So I figured I could maybe try to bridge the gap, in comes **dpgonline**.

It was built using Python, Sanic and ffmpeg. Right now it is very simple, the frontend is only basic HTML and CSS to keep bloat to a minimum. Oh and also because I do not know how to use JavaScript well nor do I care to learn about it :P

The key thing is that it works! You can visit the site, upload a video (within size limits), maybe sit in a queue for a while, and bam - you have a video that can be played through Moonshell! I have not tested this on a mobile phone which was the whole point of this... if it works there too, great.

You can try it out here: <https://dpg.deletecat.com> - I'd like to hear your feedback on [GitHub](https://github.com/deletecat/dpgonline) or [Codeberg](https://codeberg.org/deletecat/dpgonline). If you find any security issues (not missing header pish), email me at [kit@deletecat.com](mailto:kit@deletecat.com) and I'll send you 0.001 XMR or something.
