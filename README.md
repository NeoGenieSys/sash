# SASH
## Simple Adaptive Streaming over HTTP

### Overview

SASH is a new standard for adaptive HTTP streaming. SASH is inspired by MPEG DASH, and is intended to complement DASH, not replace it. Its aims are to provide a simpler, JSON based manifest format which learns from DASH's manifest design, but delivers something Javascript and Media Source Extension friendly.

SASH is implemented based on open standards as an alternative to the IP covered by the MPEG-LA DASH patent pool. 

### Design Goals
1. 100% less XML.
2. Designed for MSE and native clients.
3. Use the good parts of DASH. Skip the bad parts covered by the MPEG-LA DASH patent pool.
4. One way to do things. Follow the Python approach (There should be one -- and preferably only one --obvious way to do it.) rather than the Perl approach (TMTOWTDI).
5. Eliminate ambiguity. All client behavior should be defined. Client implementations should never guess.
6. Usable and readable. Don't make developers think. 

### Examples

* [Muxed audio and video manifest for VOD](0.1/sash-mbr-muxed-video-audio.json) (Show muxed video and audio)
* [Separate audio and video](0.1/sash-mbr-video-single-audio.json) (A fairly common real world scenario)
* [Multi angle, MBR Video, Multi language MBR Audio for VOD](0.1/sash-mbr-video-mbr-audio-multi-language-audio.json) (Multi-language audio, multiple camera angles)
* [Audio, video, and subtitles](0.1/sash-mbr-video-single-audio-single-subtitle.json) (What about subtitles?)

### How does SASH compare to HLS and DASH?

[How does SASH compare to HLS and DASH?](comparison.md)

### Is a new standard the solution?

Always.

### Is this a Joke?

No.
