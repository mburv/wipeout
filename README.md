# WipEout (PSX) Model Viewer for Google Cardboard

Built on the source code for the [WipEout Model Viewer](http://phoboslab.org/wipeout/).

## View the tracks in Wipeout like never before

* View all Wipeout tracks including 2097/XL in stereoscopic VR on Google Cardboard.

* Click the button on the Cardboard viewer to stop and look around using head tracking.

* Rotate Cardboard 90 degrees to load a random track to explore.

------

This repository does not contain the actual WipEout data files. You have to copy the `WIPEOUT/` directory from the original CD.

Building on the work of Phoboslab. More info in thier blog: http://phoboslab.org/log/2015/04/reverse-engineering-wipeout-psx


MIT License


### Known Problems

Specific to VR

 - Jarring transition when activiating head tracking

 - Fly through camera continues to move while head tracking active

 - Two unknown polygon types that are currently ignored: 0x00 (possibly padding?) and 0x0A which might be sprite-like - alpha texture, non rotated. The squiggly lights in the jump pits on Karbonis are missing; could be 0x0A?!.
 
 - The underside of the ships for WipEout have the wrong textures or UV coordinates
 
 - Fly-through Camera spline doesn't handle jumps nicely
 
 - Some faces from PRM models seem to be backwards. This only is a problem for some WOXL models. E.g. the cannopy on Spilskinake or some rocks on Vostock Island are backwards. Maybe this just didn't matter, because the original game didn't cull back faces? Or is there a flag or face normal for some polygon types?
 
