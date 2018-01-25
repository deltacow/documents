# Setup Notes

## General Info

* presenter is a walk'n'talker so Alex will be busy with his camera
* sound check will be at 3:30 -- it would be nice for us to be ready then, but it's not completely necessary as we can completely check ourselves just with Centennial staff using mics
* don't bother bringing the video streaming box...nothing is needed from it, just bring the bag of all video IO devices
* she **DOES** have a video in her Powerpoint...it's about 30 seconds long only and has no audio so we should be safe to use Desktop Presenter to get it into the stream

## Video

* standard 2 camera setup
 * wide camera should not be in centre position, but off to one side...generally we put it on the other side of the sound board
 * white balance both of the cameras to the same K value so that white looks white on the wirecast preview
 * we should also turn off auto gain control and likely auto exposure as well on both cameras, but I have used different settings for different shows...find out what works for you
* presenter will need a laptop on stage with a clicker
 * Windows is probably best
 * laptop will need to be on the same VLAN as the Wirecast setup, so you'll need to let Jim know the port it is plugged into on stage
 * install [Desktop Presenter](http://dynamic.telestream.net/downloads/download-desktop-presenter.asp?prodid=desktoppresenter) on the laptop -- because it is on the same VLAN you'll see it automatically in Wirecast as a source you can add.
 
## Audio

* Benoit and Bruce know what they normally send to you for audio, but basically:
 * get them to send you the "post fader front of house mix on 2 channels (L R)" which you'll plug in to your Behringer board as 1 and 2
 * room condenser mics will be plugged in to 3 and 4 and are phantom powered so you'll need that on on the board
* master out from the board (L & R) go to the wide camera which has the audio head set to "Line" and no auto levels

## Ustream

* Ustream username is:  XXXX
* Ustream password is:  XXXX
* there is an "event" setup on Ustream called "Maggie MacDonnell" that is the one you will use for the output of the actual broadcast.
* for testing, you'll just broadcast to the channel by itself
* channel URL is:  www.ustream.tv/channel/XXXX
* the password on the Ustream channel (for viewers) is:  XXXX

## Wirecast

* on the camera layer in Wirecast you'll have 5 total sources:
 * the wide and close cameras
 * a title card for the talk
 * the Desktop Presenter view from her laptop
 * a constructed shot that you will build, which has a small inset image in the bottom left which is the close cam, and a larger image in the upper right which is the Desktop Presenter view, see image below:

 ![Chris Hadfield inset picture](http://droplr.ubishops.ca/HZ16MH+)
 Don't worry about the logo in this picture, that was inserted by Ensemble
 
* all 5 sources on this layer should have **only** the wide camera as their audio source, ensure all others are turned off
* audio testing is done as follows:
 * connect headphones to the Behringer mixer and listen to the audio mix there
 * if it doesn't sound good at the mixer, *it will not sound good down the chain any further*
 * once you are happy at the mixer (no buzz, nothing clipping, etc) then listen to the sound at the preview side of Wirecast

![Preview of Wirecast](http://droplr.ubishops.ca/t55Ros+)

* connect headphones to the headphone jack on the Mac Pro
* all you have introduced at this point is that now the sound has been sent to the camera and is coming back from the camera
 * so, now between the master output of the mixer and the line level setting on the audio head of the camera, you just need to ensure that you are getting an appropriate audio level in Wirecast
 * generally I find that both camera channels (which have to be set to the same level) are probably going to be set to 10
 * I generally shoot for peaking at 0dB, but peaking at -6dB to -10dB will also likely sound fine on the stream
 * ensure your peaks are good, and no clipping on the audio meter in Wirecast
 * also check that when nothing is being sent (ie. master output of the Behringer is 0) you have no introduced audio in Wirecast (the meter should be right at the bottom, not registering basically anything)
 * now, start streaming on the channel, cut to a live shot in Wirecast and open the channel on another device and listen with headphones to see what the live stream sounds like (channel is at [https://www.ustream.tv/channel/bishopsuniversity](https://www.ustream.tv/channel/bishopsuniversity))
 * call Scott so he can view and listen to your livestream in his office