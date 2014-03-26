The more pictures I took, the more I learned about the color. Then I've bought a wide-gamut monitor, and then, being puzzled by the acid greens and reds, a colorimeter. That's how I've introduced myself to the [color spaces](http://en.wikipedia.org/wiki/Color_space).

Being a Linux adept for years, I started to play with [Argyll Color Management System](http://www.argyllcms.com/) and its [dispcalGUI](http://dispcalgui.hoech.net/) assistant. It had so many settings, so it puzzled me lot!

![dispcalGUI](../project_images/dispcalGUI.png?raw=true)

With the means of [iccgamut](http://argyllcms.com/doc/iccgamut.html) I've been creating VRML files for ICC profiles of my monitor and the cameras and standard color spaces like sRGB and played with them in [MeshLab](http://meshlab.sourceforge.net/). 

That's how I've learned that my monitor is capable of displaying a much lager amount of colors than it can be encoded in HDTV signal (except, probably, for some yellowish hues):

![MeshLab HDTV](../project_images/meshlab_hdtv.png?raw=true)

And that's how I've discovered that Canon 7D can capture an incredibly larger amount of colors than my monitor can display (except for some bluish):

![dispcalGUI](../project_images/meshlab_canon7d.png?raw=true)

From the article [Optics of Digital Cinema](https://www.student.cs.uwaterloo.ca/~cs781/PinhoDigitalCinemaTalk.pdf) I've learned, that cinema DLP projectors are not capable of displaying deep green colors, those inherent to film projectors. What was more disappointing is that digital cinema standard (DCI–P3) doesn't even cover 90% of the real world colors, which are described by [Pointer's research](http://onlinelibrary.wiley.com/doi/10.1002/col.5080050308/abstract).

I've also tested web browsers and figured out that Google Chrome doesn't support color management, while Mozilla Firefox does the job well.

At this point I was pretty fed by the technical details (so is the reader), and six months later, at the end of February 2014, _it_ happened.
