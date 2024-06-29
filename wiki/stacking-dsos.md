# Stacking: DSOs

### Why stack?

Stacking increase the signal-to-noise (SNR) ratio of your images. Generally speaking the noise follows fairly predictable patterns and can be removed by the use of calibration frames. This results in a smoother image - a well calibrated image is far easier to process than just a stack of light frames. Generally speaking the more frames you use, the better your image will be.

This effect does drop off however, the noise reduction depends on the square root of the number of frames we take - 25 frames decreases the noise by a factor of 5, 100 frames decreases the noise by a factor of 10 and you'd need 225 frames to decrease noise by a factor of 15.

#### Frame types

***

**Lights**

Light frames are the pictures of the image you've taken. Some stacking programs have options to select the best percentage but it's best to go through them yourself beforehand and remove any that contain unwanted artifacts such as satellite trails and streaked stars. These can influence the final image and ruin the outcome.

**Darks**

Dark frames remove the "dark signal" from your light frames. Dark signal refers to the signal that your camera is producing independent of the light entering it, and is caused by electrons which gradually accumulate in the sensor while it is exposing. To take dark frames you must cover your telescope or camera to prevent light from entering, then take a series of exposures with the same exposure time, ISO and temperature as your light frames. This enables your stacking program to subtract the dark current from your light frames reducing the noise in the final stack.

**Bias**

Bias frames remove the sum of the readout noise from your light frames. This includes all types of noise that are generated upon sensor readout, such as shot noise, read noise, camera noise (from the camera's electronics itself), interference noise, etc. Since many of these types of noise are repeatable, they can be subtracted from the light frame to reduce total noise. The best way to isolate the readout noise is to take the shortest exposure possible with the same ISO as your lights, again while covering the camera. Take a bunch (\~50) and average them together to create a master.

**Flats**

Flat frames remove defects like vignetting and dust spots from your images. To take a flat frame, cover the end of the telescope with a white t-shirt or make a flatbox, then take an exposure at the same ISO as your light frames, letting the camera decide the correct exposure time. Flatboxes will make the process easier an more accurate as they will have an evenly lit field.

#### Stacking programs

***

The most widely used stacking program is DeepSkyStacker. DSS is a very simple program, it's possible to get fine results from it with a minimal amount of effort and knowledge. It's also free and offers a basic histogram stretching functionality.

PixInsight also has an excellent stacking functionality. It can also be more advanced than DSS, allowing you to fine-tune the stacking settings to your heart's content. It generally produces better stacks, but is expensive. That said, it's also the gold-standard in post-processing so is worth buying if you have the budget.

***

#### Basic Stacking in DSS

***

This guide will focus on DeepSkyStacker since that's the most common program used. We'll assume you've checked your frames before hand, removing any satellite trails and poorly shaped stars.

1. The first thing we want to do is open and select our lights, darks, flats and bias. We then click “Check all” on the left-hand side. [DSS with images loaded](http://i.imgur.com/uNnSkxm.png)
2. Click on 'Register checked pictures' and a popup will appear. Assuming you've removed the garbage frames before hand, change the stacking percentage to 100%.
3. Next, click the 'advanced' tab on the same window, and change the star detection threshold until you get 20-30 stars. The larger the star detection threshold the less stars it will stack from. A common problem is setting the star detection too low on faint images and having DSS try to stack the noise rather than the image so it's important to get it right. [Star threshold setting](http://i.imgur.com/jj7TzHo.png)
4. Now click on “stacking parameters” on the same window. Change result to the mode you prefer (I tend to use mosaic mode). On the light tab select Median Kappa-Sigma clipping with a Kappa of 2.0 and 5 iterations. This can help to remove hot pixels and other region which fall outside of the range of signal, like satellite trails by replacing them with the median value found near them. [Kappa Sigma Clipping settings.](http://i.imgur.com/SXhUdOt.png) Everything else in the settings works OK as default, so click OK and begin stacking.
5. This will take a few minutes and it's fairly CPU intensive so it's a perfect time to have a cup of tea and a biscuit.
6. After a while DSS will preview the outcome. Click save picture to file and save it as your preferred raw format. (TIFF or FITS). You're now ready to open it in Photoshop or an alternative processing program and edit it. [Example of final stacked image.](http://i.imgur.com/LJWAz4G.png)

#### Basic Processing in DSS

***

A proper processing workflow is outside of the scope of this particular article. I have however written a quick guide to histogram stretching in DSS in the past, so I will include this. It's really no substitute for Photoshop or PixInsight though.

As an example of DSS's capabilities, here is a short processing workflow courtesy of /u/yawg6669

1. [Output of stacked images, pre-processing](http://i.imgur.com/Z9RBDsb.png)
2. Next, the [R/G/B channels are aligned](http://i.imgur.com/fdvv3wK.png) using the provided sliders and applied.
3. Next, move over to the 'Luminance' tab, and adjust the midtones. It'll take a bit of playing with but generally you will want to make the curve a little steeper with the top slider then move it across the RGB range until it looks good. Moving the slider to the right will darken the image, moving to the left will brighten it. [Here's how it looks after adjusting the Luminance.](http://i.imgur.com/DKlS2oL.png)
4. Move to the Saturation tab and up it until you get some colors you like. This is a personal preference thing, I like mine around 20 though it'll depend on your conditions and camera. [Image after adjusting Saturation.](http://i.imgur.com/M5oQkyz.png)
5. If you want you can go back into the Luminance tab and play around with the Darkness and Highlight sliders - these do pretty much what they say, influencing the brightest and darkest parts of the image. Again you'll need to experiment with them to find out what gives a good result. [After decreasing the highlights and increased the darkness](http://i.imgur.com/86MB73F.png)
6. [Finally, export the final image.](http://i.imgur.com/ffYXLkO.jpg).

As you can see there's gradients, vignettes and stacking artifacts all over the place, but it's better than no post-processing at all. For comparison, [here's the same image processed in PixInsight.](http://i.imgur.com/cgmRL6Z.jpg)
