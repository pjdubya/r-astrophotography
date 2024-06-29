# Filters

_Written by /u/yawg6669_

### The nature of light

For those unfamiliar with chemistry or physics, this section is a brief outline about light. When doing astrophotography, there are essentially two types of light being captures, infrared (IR), and visible (Vis). Visible light is the light you can see with your eyes, the light that gives “color” to things, red apples, green grass, blue sky, etc. IR light is light that is at a lower energy than visible light, and therefore has some different properties. IR light cannot be seen with the human eye, and therefore we need to use a camera of some sort to capture it. The energy of light is dependent upon its wavelength, where a longer wavelength corresponds to a lower energy. Figure 1 shows a spectrum of light that includes the wavelength labels.

> Figure 1: Visible light spectrum and corresponding wavelengths.

As seen in figure 1 the color “red” as we know it isn't really a single color (i.e. a single wavelength), but rather a grouping of wavelengths around the 650-700nm area of the spectrum. This is important because later on when talking about filters, we will be “chopping” up the red spectrum into different parts, some of which can be imaged from a one shot color camera (like a DSLR), and some which cannot.

### How a One Shot Colour Camera works (DSLRs, Mirrorless, Colour Astro cams etc)

A one shot colour (OSC) camera essentially contains a digital sensor paired with a colour filter array (CFA) ontop of it. The CFA is what allows the camera to take a color photograph. The job of the digital sensor is simply to record the arrival of photons regardless of wavelength/colour. If a red photon is to be recorded, a “red filter” must be used, one that only allows “red light” (i.e. light that has a wavelength between about 600-700nm) through. If a green photon is to be recorded, a “green filter” must be used (\~500-550nm), and the same goes for a blue photon (\~450-500nm). It is this three color scheme that allows full color images to be captured by the camera. Therefore, for this to occur, the camera itself must have these filters built into the camera, and they do. Most OSC cameras contain a particular CFA called the Bayer filter which composes a 2x2 square to cover a single pixel, a noticeable exception is Fujifilms recent X-Trans sensor with their own X-Trans CFA. One can remove the CFA from their camera to acquire monochrome or “black and white” images via physically scraping it off.

### How a Mono Camera works

Monochromatic or mono cameras are simply cameras with just the digital sensor without the CFA layer on it. They're typically more expensive than colour cameras presumably due to the smaller market for sensors without the CFA. When imaging with a mono the astrophotographer must intentionally acquire a series of images with different filters if a color image is desired. Lack of any filters will result in a “black and white” image, where each pixel is simply recording how much light it absorbed, regardless of the wavelength of that light. This brings us to filters, the topic of this section.

### Filter types

There are two main distinctions between filters used in astronomy, those that are used to see things (visual filters), and those that are use to help image things (photographic filters). Since this is an AP subreddit, only photographic filters will be described here.

When imaging with a non-modified DSLR (or any OSC cam for that matter), light is already being filtered into wavelengths by the CFA and so no additional filters are necessary. Of course, since many of us live in light polluted locations, “light pollution filters” are often used. A light pollution filter is a photographic filter designed to remove certain wavelengths of light that are common in areas of civilization. Because many towns use mercury and sodium lights to light their streets, houses, parking lots, etc, the amount of light around is typically flooded by wavelengths of light that match that of mercury (chemical symbol: Hg) and sodium (chemical symbol: Na). Since intelligent chemists have figured out which wavelengths those are, other intelligent people have found a way to filter them out using a light pollution filter. See figure 2.

> Figure 2: Figure 2: Light pollution lines and common filters, Baader.

Figure 2 is complex, but focus on the orange lines. The orange lines in figure demonstrate which specific wavelengths of light are given off by mercury (Hg) and sodium (Na) lights. Therefore, when using a light pollution filter, such as the Baader UHC-S filter shown as the blue line in figure 2, the amount of light that gets past the filter and makes it to the sensor is essentially 0 for many of the mercury and sodium wavelengths (such as 546nm, 577nm, 578nm, etc). This is how light pollution suppression works.

Of course, one could always add a more than one filter in front of a OSC camera. OSC cameras often come with more than one filter built in. We have already seen how they must include a Bayer array (otherwise they wouldn't be a OSC camera), but many also include an ultraviolet (UV) IR cut filter.

#### UV-IR cut filters

***

A UV-IR filter is a filter designed to limit the amount of light that makes it to the sensor to a certain predefined area of the visible and infrared spectrum. Recall figure 1. There is still plenty of light that has a wavelength less than 400nm (we call this ultra-violet), or greater than 700nm (we call this infrared, sometimes referred to as “deep infrared” or “deep IR”). Since the astrophotographer likely does not want this light to hit his/her sensor (for various reasons that are beyond the scope of this entry), it needs to be filtered out. That filtering is done by the UV-IR cut filter. This filter is a single filter that, just like a light pollution filter, will not allow light with a wavelength less than 400nm, or greater than 700nm to pass. Therefore, all light that DOES pass through this filter must be in an appropriate wavelength range, which is what the astrophotographer desires. There are many UV-IR cut filters available, many of which will “cut out” light at different values. For example, some will allow light of 699nm to pass, but 700nm is not allowed, while other filters will allow 700nm to pass, but 715nm is not allowed. The varying values of the “cut off” point is a user selectable option.

Of course, there is no reason the UV-IR cut filter must be one piece of glass. It is completely possible to only use an IR cut filter which will “cut out” all IR light (i.e. light with a wavelength greater than 700nm), but let all light less than 700nm pass. The same can be said for the UV side of the spectrum.

#### Broadband vs Narrowband

***

When imaging with a mono camera, there are two main methods by which to obtain color. One method is through “broadband” imaging (also called RGB imaging), and the other is through “narrowband” imaging. In a broadband image, color is collected through filters that are provided by the astrophotographer, and mimick the Bayer array. The color filters used are red, green, and blue. Broadband imaging provides a significant increase in resolution of a given sensor, because during an exposure the entire chip is being utilized to collect the light. In a OSC camera, only the pixels under a given color are being used, which, depending on color, is 25% or 50% of the total number of pixels. So, by broadband imaging with a red, green, and blue filter, you are increasing the effective resolution of your image by 25%, 50%, and 25%, respectively, as compared to a OSC camera with the same sensor. Of course, using this method, the filters need to be purchased and maintained separately from the camera, more for the astrophotographer.

Narrowband imaging is an entirely different technique. Whereas broadband imaging says “I'm going to collect ALL wavelengths of light between 600-700nm and call that red” in order to get color, narrowband imaging says “I'm going to pick ONE wavelength, say 656.3nm, and call that red.” Therefore, when narrowband imaging, the astrophotographer is essentially picked one wavelength of light he/she would like to record, and providing a filter that does exactly that. The most common wavelength of light that is imaged in this method is hydrogen alpha (Ha) which gives off light of 656.3nm. There are many astronomical objects that give off this light, and so there are many “Ha” targets available for a narrowband imager. Unfortunately, since this light is limited to a single wavelength, often very long exposures are needed in order to collect enough light such that the signal to noise ratio is high enough to generate a good image. This is why an expensive, high quality, mono-CCD is used with narrowband imaging. Other common narrowband wavelengths are shown in figure 2, such as oxygen three (OIII) at 495.nm, and 500.7nm. Do note there is some 'width' to which what wavelengths a narrowband filter lets through. I.e. 7nm, 3nm.

#### Planetary Filters

***

As with deep sky imaging, planetary can also be done with either an osc camera or mono. Some OSC cameras such as the ASI 224MC offer high IR sensitivity which can be of benefit. When imaging the moon and not intending to saturate the soil colour, an IR Pass filter may be employed to cut through the worst of the atmospheric seeing which affects the bluer end of the spectrum. Alternatively you may require an IR cut filter when imaging mars if you wish to attain colour accuracy.

Other specialty filters also exist such as Ultra violet bandpasses, or Methane CH4. These allow for imaging of specific cloud structure detail in planets which may not be otherwise visible in broadband RGB.
