# Stacking: Planets

### Why stack?

Solar system imaging is fairly similar to DSO imaging in that we want to combine good images together to increase the signal to noise ratio. As planets are so bright and affected by atmosphere the best way to do this is by trying to get as many frames of them as possible with a high FPS video. This overcomes the effects of atmospheric turbulence and allows us to stack many good quality frames.

Solar system imaging is a good way to get into astrophotography if you're coming from a visual setup or don't want to commit to spending thousands of dollars on a deep sky rig just yet, as you don't really require tracking and the large aperture of dobsonians and the like are well suited to resolving fine detail on the planet's surface.

#### Capturing your image

***

As mentioned, planetary works best with high FPS capture and good seeing so we take short videos of the planets. As mentioned, how long these videos can be depends on the rotational periods of the planets, which is why high framerates are beneficial. Videos can be captured using capture programs such as Sharpcap or Firecapture. Getting the gain and brightness at the correct level is important as it influences both the FPS and the noise levels of the final image. It is easy to overexpose bright crater rims and features while imaging the moon so be mindful of this.

#### Image rotation

***

Planets rotate. That may seem obvious, but rotation can have an effect on the level of detail you see in your images. This also means the length of time you can spend capturing video before rotation becomes obvious is limited with some planets, most notably Jupiter and Saturn which take around 10 hours and 10½ hours respectively. This quick rotation combined with their large size can make rotation noticeable even after only 60 seconds.

Rotation can be corrected with WinJupos, which is an excellent tool but out of the scope of this beginner's guide.

#### Calibration frames

***

Calibration frames are important for planetary as with DSOs. Flats are very useful for removing giant dust spots, especially on lunar and solar images, which make stacking inaccurate. Similarly, darks are useful for dealing with noise.

Flats can be taken in a similar manner to how you would take them for deep sky, i.e. putting a white sheet over the end of your telescope and adjusting the camera exposure until it isn't overexposed. You can also take flats by defocusing your telescope and pointing at the moon. You can then take a short (30 seconds is fine) video, and import it into Autostakkert. From there, select "image calibration" and select "create a master frame". You can then save it as a flat TIFF.

Darks are also taken in the same manner as DSO darks, i.e. by covering the telescope and taking a short video with the same settings as your lights. Do the same as you did with the flat frame in Autostakkert, and save it as a dark TIFF.

#### Stacking

***

For stacking we recommend using Autostakkert over Registax, as it tends to give better results. Import your video and calibration frames and choose the settings which work best for you. You can then press analyze and stack a suitable number of frames from your video. This depends on seeing, but typically will be less than 50%. More frames give less noise but a less sharp image whereas less frames will increase noise but also increase detail.

#### Wavelet Processing

***

One thing Registax is _excellent_ at is processing your planetary images. Registax wavelets are a great tool and work by sharpening the details in your picture. Using linked wavelets is the best way to get good detail out of an image, if you keep practicing you will get a feel for how they work and be able to use them effectively to produce excellent images.

[There is an excellent guide on Wavelet processing located here.](http://www.astronomie.be/registax/linkedwavelets.html)

### Stacking Software

[Registax](http://www.astronomie.be/registax/download.html)

[Autostakkert](http://www.autostakkert.com/wp/download/)

[WinJupos](http://jupos.org/gh/download.htm)
