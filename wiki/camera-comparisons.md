# Camera comparisons

In astrophotography you'll find a wide range of cameras being used by hobbyist, and you'll see several terms flung around such as CMOS/CCD/DSLR or astro camera.

To get some acryonyms out of the way here is a brief definition on some cameras:

* Digital Single Lens Reflex (DSLR) refers to a common consumer camera form factor which involves a small mirror that flips up to direct light to the view finder for framing. i.e. Canon 60D. In contrast there is also DSLM or Mirrorless cameras that lack this mirror, i.e. Sony A6000.
* Astro camera refers to a camera dedicated to astronomy, these typically require a computer connection and do not have any buttons or displays. (i.e. ZWO ASI 1600)

### CCD & CMOS Distinction

Charged-coupled Device (CCD) and Complementary metal–oxide–semiconductor (CMOS) refer to two different sensor technologies that are commonly found today. CCDs have been around since the 70s, where as CMOS was only developed by 1993 and only within the last two decades has CMOS started to dominate the market.

Both sensor technologies have been found in all types of cameras (DSLRS and astro cameras), astro cameras historically were all typically using CCD sensors up until around 2010 when more affordable CMOS cameras hit the market. Most consumer cameras (DSLRS and astrocams) now typically use CMOS sensors as the technology continues to mature and improve.

Up until recently, CCDs typically offered better [Quantum Efficiency](http://en.wikipedia.org/wiki/Quantum\_efficiency) (QE, effectively a measure of sensitivity), dynamic range with a 16 bit adc and larger full well depth. CMOS cameras in the market are starting reach similar capabilities with technologies such as dual gain, back side illumination (BSI), and through the use of 16 bit adcs too. However this comparison should be made between specific cameras.

CCDs work by having a single analog to digital converter (adc) to convert accumulated electrical charge into a digital number, this means the read noise distribution is constant. CCD read noise root mean square (rms) is typically higher than cmos sensors. In addition to this readout method, it allows for hardware level binning, where charges from multiple pixels i.e. a 2x2 square, can be accumulated together before the adc achieving an improved signal to noise ratio (SNR) with a loss in resolution.

CMOS however work by having amplifiers on each pixel, and an adc per column of pixels, therefore each column of pixels will most likely have a slightly different distribution of read noise. (This is one reason why the scientific crowd is slow to adopt CMOS as this can impact measurements). Historically CMOS had a worse QE due to the fact each pixel had a bunch of amplifier circuitry on the front occupying its surface area, BSI is an improvement on this, that moves this to the underside, allowing for more photons to be collected.

#### Advantages of DSLR/DSLMs

***

* DSLRs are typically much less expensive than astro cameras, especially when all the astrocameras's accessories and filters are included.
* DSLRS work standalone, does not require a computer to be used, for some setups this may prove useful.
* DSLRs can come off the telescope and be a 'camera' when you're not imaging.
* Can use the cameras lens system easily

#### Advantages of Astro Cams

***

* May offer Cooling
* Mono or OSC choice
* Typically CFA and other filters optimised for astro wavelengths (no ir filters) \*
