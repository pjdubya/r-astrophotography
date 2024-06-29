# Polar Alignment

To start the polar alignment article, let's go into a brief overview of _what_ polar alignment is. Put very simply, polar alignment is aligning the right ascension axis of our telescope mount with the rotational axis of the earth.

Unguided telescopes track on a single axis (the R/A). This works by moving the telescope at a constant sidereal rate to counteract the way the earth is moving. The mount doesn't know that it's not aligned, it will move at the sidereal rate regardless of where the R/A axis is pointing. This is why it's important to align it with the rotational axis - so it can effectively track the stars.

[For an interesting video on the basics, click here.](https://www.youtube.com/watch?v=plx6XXDgf2E)

### Effects of Polar Alignment

A bad polar alignment causes the stars to trail in your image. This will make or break your imaging session, if you can't polar align your mount you won't be able to get good images. An average unguided mount can accurately track for several minutes using a small telescope provided it has a good polar alignment. Even if you guide your mount a bad polar alignment will cause field rotation to occur since it will compensate for the R/A error with declination axis tracking.

[This image was taken with poor polar alignment](http://i.imgur.com/ZgWR2na.jpg) - The sub-exposures are only 30 seconds long and still show trailing.

[This image was taken with a better polar alignment](http://i.imgur.com/pLoBSSy.jpg) - The same mount was able to track accurately for 120 seconds without trailing.

### Polar Alignment Methods

There are many methods you can use to polar align your telescope - they're all fairly useful and will get your mount to a good enough alignment that you can image with it if done correctly. Each have their pros and cons however - some take a long time, some are less accurate, etc. Each work toward doing the same thing however - aligning your R/A axis with the earth's rotational axis. We've included some of the more popular ones here for you to try out.

#### Drift alignment

***

To understand drift alignment it's important to understand what we're doing, why we're doing it and what we're trying to achieve. Drift alignment seems to be the form which most often confuses an puts off beginners into the hobby. It's actually fairly simple once you understand it.

The fundamental basic of polar alignment is that we're trying to align the R/A (Right Ascension) axis of the telescope with the axis that the earth spins upon. We can adjust the R/A axis in two ways - from side to side (the azimuth adjustment) and up and down (the altitude adjustment). This is kind of similar to how a dobsonian telescope works - the alt and az bolts are two pivot points with which you point your R/A axis similar to how a dobsonian uses two pivot points to point a telescope.

This is shown on the diagram below - the R/A axis is marked in red, the azimuth pivot point is marked in pink, and the altitude pivot point is marked in blue. On most mounts there are screws to adjust these.

In drift alignment we start with the azimuth adjustment.

**Azimuth adjustment**

In the azimuth adustment we are trying to get the side-side alignment of our R/A axis right. Set up your mount as normal, use the polarscope or a compass to get it pointing fairly close to North. Turn on your telescope and get to a point where it is tracking the stars. You don't need to do any star alignments for GOTO functions at this point.

Next, use the handset to point the telescope at a star which appears to be near the meridian, south of your telescope. Watch the star through an eyepiece or BackyardEOS's live-view (it has a really handy drift align reticle for this purpose where you can zoom in). Watch for motion in the star. Assuming you're not super lucky and haven't managed to point the mount due north to start with there should be some movement (drifting) visible in the star. The motion of the star tells us how well our mount is aligned.

If the R/A is too far East the star will appear to move North in the field of view.

Look at the path of the star (black arc) in relation to the path of our field of view (thick red arc) in the image below. The path of the star goes _up_ through our field of view. You can get an idea of which direction is up or down by shining a small flashlight across the front of your telescope. Adjust the mount accordingly to point the R/A further west until movement stops.

If the R/A is too far West the star will appear to move South in the field of view.

Again, look at the path of the star (black arc) in the image below. The star appears to move _down_ through our field of view, toward the southern pole. Adjust accordingly to point the R/A further east until movement stops.

Once we've got the azimuth alignment correct the star should no longer show movement in the field of view. This type of alignment can be very precise, but can also be quite time consuming to get dead-on. The image below shows the path of the star in relation to our field of view when the alignment is dead on.

**Altitude adjustment**

Once azimuth movement is minimized or stopped, point the telescope toward a star in the eastern sky (the western sky will work too, just reverse the directions given here). As with the azimuth adjustment if the R/A axis is not sufficiently angled the star will appear to move through the field of view.

If the star moves south in our field of view the R/A axis is pointed too low. As with the azimuth adjustment the path of the star moves according to the earth's rotational axis. In the image below you can see how the path of the star (black) moves through our field of view (red). Adjust the mount to increase the angle of the R/A axis until movement slows or stops.

If the star moves north in our field of view the R/A axis is pointed too high. Adjust accordingly until movement stops.

Once alignment is dead on the mount will be able to track the star without it moving in the field of view. See in the image below how the earth's rotational axis and our mount's R/A axis are aligned, therefore the tracking can follow the star.

And now we're hopefully done with drift aligning! If you're unable to get movement to stop completely in your first run through, you can repeat the process several times until you're happy with it.

#### Camera Drift alignment

***

Camera drift alignment (also known as "DARV") is a streamlined way of regular drift alignment using your DSLR or CCD to speed up the process. This allows a similar degree of accuracy, just with less time spent watching and waiting for the star to move around the field of view.

[An excellent guide to camera drift aligning can be found here](http://www.cloudynights.com/page/articles/cat/articles/darv-drift-alignment-by-robert-vice-r2760)

#### Handset routines

***

Many modern mounts have a polar alignment routine built into the handset. Celestron use ASPA (all-star polar align) and Skywatcher use a polar align based on the corrections made while 3-star aligning for GOTO function.

To get into the Skywatcher polar alignment set up your mount as normal. Go through the 3-star GOTO alignment procedure, then go back into the alignment menu and a "Polar align" option should have appeared at the bottom. Follow the instructions displayed on the handset, then do another 3-star alignment to get the mount's GOTO accuracy back. You can repeat the polar align function as well to improve the accuracy. This is one of the easier ways to align and can be completed accurately in around 5 minutes.

The Celestron ASPA routine is [explained here on the Celestron website](http://www.celestron.com/university/astroimaging/all-star-polar-alignment).

#### Electronically-assisted polar alignment (SharpCap, PoleMaster)

***

A more modern technique which has emerged in the past few years is electronically assisted polar alignment. This uses hardware and software to accurately calculate where your RA axis is pointing and gives easy to follow directional instructions on how to adjust it. There are a few vendors offering tools to polar align, however in the interests of brevity we will cover two of the most popular; SharpCap and the QHY PoleMaster. SharpCap is the cheaper method, PoleMaster is the more expensive, but both work around the same principle.

To perform SharpCap's polar align procedure you will need a supported camera, a telescope or guidescope with a field of view between 0.5 and 2.5°, and the SharpCap Pro software (£10/year license circa 2018). The software uses the camera to plate solve and calculate the location of the pole, then give instructions on where to move the axis. [A full guide can be found on the SharpCap page](https://docs.sharpcap.co.uk/2.9/15\_PolarAlignment.htm).

To use the PoleMaster requres the PoleMaster camera (around £280), an adapter for your specific mount, and the included software and cables. It is possible to hack the drivers for the QHY5L-II camera if you already own one and use that instead as they use similar hardware, but we won't cover that here. To use the PoleMaster alignment you select a star in liveview, rotate the axis so the software can calculate the NCP, then adjust the mount until the RA is pointed at the NCP. [You can read the PoleMaster manual here](https://www.firstlightoptics.com/user/manuals/polemaster\_user\_manual\_english\_UK\_northern\_hemisphere.pdf).

#### Platesolving, Simulated Drift

***

Astrotortilla & [NINA](https://bitbucket.org/Isbeorn/nina/wiki/Home) can be used to plate-solve for a very accurate polar alignment. Either program captures a quick frame of the sky, plate solves it to work out what it is, then slews the mount in R/A and captures another frame. This is a similar principle to drift alignment - the two frames should be along a predictable path followed by the R/A tracking, if the alignment is off then the platesolve will discover where the second frame is in the sky and direct you to adjust the mount accordingly. This has the advantage of giving precise numbers (in degrees, arcminutes and arcseconds) of exactly how far you are away from a proper polar alignment.

Setting up Astrotortilla properly for plate solving is a fairly involved and complicated process and [a guide to doing so can be found here](http://lightvortexastronomy.blogspot.co.uk/2013/08/tutorial-imaging-setting-up-and-using.html). Additioanlly, a basic control guide to [NINA's polar alignment method can be found here](https://bitbucket.org/Isbeorn/nina/wiki/Home).

***

#### Polar alignment scopes

***

/u/plaidhat1 on Reddit contributed the following directions of use of the Orion Sirius's built-in Polar Alignment Scope. While these directions are specific to that mount, they are a good practical set of guidelines for using any polar alignment scope. The process will be generally the same for most mounts and PA scopes. Using a PA scope, of course, relies on both the quality of the scope, and the accuracy of your mount's alignment with the scope. A well aligned quality PA scope can certainly give you a polar alignment capable of tracking stars for several minutes. Be aware, however, that even the best equipment and alignment will still be less accurate than the results offered by precise drift alignment. /u/plaidhat1

> I regularly run my Sirius EQ-G for 3 minutes, unguided, without it showing up too badly in my shots. There are two main things I'm trying to do when I set my mount up:
>
> 1. Make sure the mount is level.
> 2. Make sure it's aligned with Polaris.
>
> Here's what I do to accomplish that:
>
> 1. Set up the mount and point it approximately toward Polaris.
> 2. Make sure that the mount is level. I have a plumb-bob app I use for this purpose. I set my phone on the accessory tray with the Y-axis of my plumb-bob app aligned with North leg and the X-axis aligned with the other two legs. Adjust the North leg and one of the other two legs until it's level. I try to be within ±0.1°.
> 3. Release the Declination lock lever. Point your scope toward the horizon and lock it there. We're going to want to use the polar alignment scope built into the mount, and to do so we need to make a hole in the declination axis (which you may not have seen yet) line up with that scope. Pointing your scope toward the horizon should do that. Oh, you'll also need your counterweight shaft extended to see through the polar alignment scope at all.
> 4. Take the cap off the front opening, and the cover off the polar alignment scope. (It's possible to put these things back on the mount in the dark, but it takes a little practice with the cap to get the threading right)
> 5. Look through the polar alignment scope. You may need to focus it. Hopefully you've got your mount pointed close enough to Polaris that you can see it in the polar alignment scope's field of view. I prefer to have my mount powered off when I do this, since when it's powered on, there's a light that comes on for the polar alignment scope and drowns out my view of the star. Still, there's a really useful diagram that you'll want to see to conduct the alignment properly. I usually hold my phone up next to my eye or in front of the front opening, and give myself just enough light to see this diagram without drowning out Polaris.
> 6. The diagram shows the Big Dipper and Cassiopeia, and a little circle on a big circle which marks where Polaris should be. Grab your scope and release your right ascension lock, then tilt the mount until the Big Dipper (or Cassiopeia, whichever is in season) looks like it is where it ought to be. Now you need to get Polaris into the little Polaris circle. Move the mount around until Polaris is aligned with that circle in the horizontal direction, then use the latitude adjustment knobs to move it up or down until it's right in the center of that little circle.
> 7. Go back to step 2 and run through this procedure until you don't need to make any further adjustments.
> 8. Put the cap and cover back on, turn the mount on, and go through your normal 3-star alignment procedure.
>
> I've tried to use much of the same terminology here that Orion does. If you load up the Sirius EQ-G manual (PDF) and flip to page 5, that should make it easier to figure out what I'm talking about if you have any questions.
>
> Warning: Never stick your finger through the hole in the declination axis. If something happened and your scope flipped around on you suddenly, it would be a very bad day for you and your former finger.
