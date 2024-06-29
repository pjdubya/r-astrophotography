# Autoguiding

### Welcome to Autoguiding!

Autoguiding is an incredibly valuable tool for the Astrophotographer of all skill and equipment sets. If you own an equatorial mount, (no matter what kind you own), autoguiding is essential for ensuring your exposures come out crisp and streak-less. Autoguiding can bring you from only being able to shoot for a max of 2-3 minutes, to being able to shoot indefinitely long exposures.

### How it works

While your main camera is taking pictures in the span of minutes, your autoguider is taking pictures every second or two depending on your settings. The autoguider looks for changes in the position of your guide star, and relays corrections to be made to your mount. Since this is updated every second, your main camera is kept on target over the course of the image.

Before you start your imaging session, you have to calibrate the guider with your mount. Software tells the mount to move a certain amount of steps in 4 different directions, and the software logs the average movement between each step so it knows what to do when your star moves on its own later on.

The number of calibration steps depends entirely on the focal length of your guidescope and the type of guide camera you are using. Luckily, PHD2 can help you with these settings. Just use the "New Profile Wizard" to set up your software with your equipment. The wizard will ask you your guide camera, its pixel size, and the focal length of your guidescope. In my case, I use the Lodestar X2, so I would tell PHD my pixel size is 8.2 um. This may be different depending on what camera you are using. Afterwards, it asks what kind of mount I am using. I would select the Ascom driver for EQ6r, but again, it may be different in your case depending on what kind of mount you have.

It then asks for your guide-speed, which is usually default at .5 sidereal rate. If you have an encoder in your declination axis, select the button asking if you have one. If not, don't select it. Continue setting up your profile and name it. If you are set up in a permanent location, you can select "auto restore calibration" if you do not move / tear down your setup after the calibration. You may also choose to build a dark-library so PHD can get rid of noise inherent to your camera. This is very useful, as the software cannot tell between a hot-pixel and an actual star. If you are guiding on a hot-pixel, you will not actually be guiding on a star, and your images will come out just as if they weren't being guided at all.

Autoguiding isn't infallible, and both you and experienced imagers _will_ experience issues with your guiding occasionally. Exterior forces such as wind and other vibrations can cause your guiding to not work as accurately as it should. Even with a perfect polar alignment, mechanical imperfections in the gears will not allow you to shoot unguided for more than a few minutes.

***

### Autoguiding Options

Separate Guidescope and guide camera.

* Pros: Easy to set up and use.
* Cons: Flexure, additional weight.

Off Axis guider - Uses a prism to split off a bit of light from your main imaging telescope. Doesn't affect main imaging sensor.

* Pros: More accurate.
* Cons: More expensive, harder to find a bright guidestar. Needs a sensitive camera.

Dual-Chip camera.

* Pros: Easy to set up and use.
* Cons: Expensive!

***

### Recommended Autoguider Setups

#### Cameras

We no longer recommend the StarShoot Autoguider. It is simply too noisy, and too expensive compared to newer competition. A newer ZWO camera can be half the price, more sensitive, with a much better noise profile.

* ZWO ASI120MM-Mini
* ZWO ASI290MM-Mini
* ZWO ASI 174MM-Mini
* QHYCCD QHY5L-II
* Starlight Express Lodestar
* Starlight Express Lodestar x2

If you have a planetary imaging camera, whether it be color or mono, give it a try before you buy something else.

#### Guide Scopes

Be sure to buy tube rings if they aren't included. You'll need them to attach the guidescope to your main imaging scope.

* Agena 50mm Deluxe Straight-Through Finder / Guidescope
* Agena 60mm f/4 Precision Straight-Through Finder / Guide Scope
* Orion CT80
* Orion Mini 50mm Guidescope
* Orion 60mm Multi-use Guidescope
* ZWO Mini Guidescope

Any of these guidescopes will work well with any of these cameras.

In our opinion, the best bang for your buck will be with an Agena 60mm Guidescope with a ZWO ASI 120MM-Mini. The total cost of this setup is less than a single Starshoot Autoguider.

As we have said, do your research. You may find a guidescope cheaper than any of these that will work just as well. If you have any questions, feel free to ask them on /r/AskAstrophotography or our [Discord chat](https://discordapp.com/invite/WPD7Jn2).

### Things to keep in mind

The ratio of your imaging scale is an important factor to consider when deciding on an autoguiding setup.

Here is a handy formula to figure this out.

Formula should look like this:

* F = Ratio of image scale of both guidescope and imaging scope
* S = size of camera pixels
* FL = Focal Length of telescope

F = S(guidecam) x FL(imagingscope) / S(imagingcam) x FL(guidescope)

You ideally want your F ratio to be "1", though anything up to a ratio of 3 should work. Ideally, your guidescope focal length should be atleast 1/3rd of your main scope.

***

For a more detailed description on how to use autoguiding, refer to [PHD2's website](https://openphdguiding.org/manual/?section=Basic\_use.htm#Guiding)

They have a lot of information on how guiding works, how to set it up, and have a lot of answers to common guiding and calibration issues, [located here](https://openphdguiding.org/manual/?section=Trouble\_shooting.htm).

We recommend the use of ASCOM and EQMod control and the use of a serial to USB cable connected to the hand controller. You can also make or buy an "EQDIR" cable, which cuts out the need for the hand controller. This is only recommended if you use plate solving instead of a 3-Star alignment. The Autoguider can be plugged in to your computer via USB. ST4 is not considered to be a great option, as you will need to recalibrate your guiding every time you slew your telescope.

### Required Software

[EQMod](http://eq-mod.sourceforge.net/)

[Ascom](https://www.ascom-standards.org/)

[PHD2 (Push here Dummy 2)](https://openphdguiding.org/)
