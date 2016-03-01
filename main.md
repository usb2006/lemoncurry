# Open Source Photopolymer DLP 3D Printer #


---


A UV or visible light sensitive monomer is used for three-dimensional printing called microstereo lithography. Using a DLP video projector with a UV output, it is able to create incredibly thin polymer layers and build objects layer by layer. The initial design howto will have movement for building vat grown models in the z-axis only.

**This design already works in a laboratory environment with lab grade equipment.** The object of this design is to offer a GPL open hardware howto that anyone with opposable thumbs and moderate thinking abilities might reproduce in the privacy of their own parents basement.

**IRC Freenode [#3dprinters](irc://irc.freenode.net/3dprinters)**

The next generation UV Photopolymer DLP 3D Printer project will be laser based and be capable of printing submicron features for the microfabrication of very small micro-machines and mechanisms.

Several resins are available in various chemistries from under $40/L (<$40/Kg) and up depending on chemistry and performance.

Cure rates are be possible under 0.2 seconds per layer or slice. This allows for build rates over 1 inch per minute.

Layer thickness maybe be any range you wish from 1um to 250um based upon the resin and lamp used.



UV http://en.wikipedia.org/wiki/UV

Photopolymer http://en.wikipedia.org/wiki/Photopolymer

DLP http://en.wikipedia.org/wiki/Digital_Light_Processing

3D Printer http://en.wikipedia.org/wiki/3d_printer

Lemon Curry http://www.youtube.com/watch?v=qKhit2nsoq4


---


**System Diagram**

![http://lemoncurry.googlecode.com/files/lc01.jpg](http://lemoncurry.googlecode.com/files/lc01.jpg)

(2D Rendering, not a photo)


---



**Z-Axis Animation**

http://code.google.com/p/lemoncurry/downloads/detail?name=lc00.avi&can=2&q=


---


**Sample DLP Prints**

![http://bucktownpolymers.com/images/carprint00.jpg](http://bucktownpolymers.com/images/carprint00.jpg)

![http://bucktownpolymers.com/images/carprint01.jpg](http://bucktownpolymers.com/images/carprint01.jpg)

80mm Toy Car Bodies, 10um layers (actual prints, not renderings)
Some people have been confused with what printer was used for these prints. Lemoncurry is not a printer or printer kit, it is a howto for building these types of printers. These prints were made with this type of SLA printer.


---


## Photopolymers ##

UV and Visible Light Cured

Polyester, Vinyl Ester, Urethane, Acrylics

Epoxy, ABS, Styrene, Oligomer, Silicone

Waterborne Emulsions

Several colors and effects such as pearl, metallics and stone.

For light sources with a wide spectrum of output many types of photopolymers maybe used. Photopolymers however tend to have a narrow range of spectral sensitivity for the initiation of polymerization. The most efficient designs match the spectra of the light source to the peak sensitivity of the photopolymer.

**UVA Cured**

Many DLP projectors use Mercury Lamps that output some UVA in the 385-400nm range. 385nm photopolymers are sensitive to UV light just outside the visible spectrum and may be handled indoors without them hardening. They should be kept from exposure to sunlight, bright mercury vapour lamps or other UV sources.

http://bucktownpolymers.com
Several chemistries are available in Cyan, Magenta, Yellow, Black and White.

The viscosity of these photopolymers may be varied greatly by controlling their temperature while printing. A heated vat is necessary for a low viscosity. A runaway heater safety circuit is recommended to avoid fire or overheating.

Photopolymers below 385nm do not make good candidates for DLP printers since the shorter wavelength UV light required for curing rapidly deteriorates the sealants used in most DLP's.

**When sunlight reaches the surface of the earth on a sunny day the level of 385nm UV is around 0.03W/sq cm. This is the minimum level to try for at the surface of the UV photopolymer with a DLP projector. At this level curing will be slow but it will cure. Higher levels will make polymerization occur faster. Some systems attain 100W/sq cm and cure very rapidly.**

**Visible Light Cured**

http://bucktownpolymers.com/polymer01.html Several chemistries are available in Cyan, Magenta, Yellow, Black and White.

The viscosity of these photopolymers may be varied greatly by controlling their temperature while printing. A heated vat is necessary for a low viscosity. A runaway heater safety circuit is recommended to avoid fire or overheating.

405nm and above photopolymers are sensitive to light within the visible spectrum and should be handled away from sunlight or bright lights.

405nm is the wavelength of LED lasers found in Blue Ray drives.

470nm Blue Led's are available in a wide range of power levels and beam angles.



---


## Electromagnetic Spectrum ##

![http://www.giangrandi.ch/optics/spectrum/em-spectrum-a.jpg](http://www.giangrandi.ch/optics/spectrum/em-spectrum-a.jpg)

![http://media-1.web.britannica.com/eb-media/30/27030-004-293E0372.jpg](http://media-1.web.britannica.com/eb-media/30/27030-004-293E0372.jpg)

**UVA to IR**
![http://www.giangrandi.ch/optics/spectrum/visible-a.jpg](http://www.giangrandi.ch/optics/spectrum/visible-a.jpg)

| **Name** | **Abbreviation** | **Wavelength Range in Nanometers** | **Energy per Photon** |
|:---------|:-----------------|:-----------------------------------|:----------------------|
| Ultraviolet A, long wave, or black light | UVA              | 315 nm–400 nm                      |3.10–3.94 eV           |
| Near     | NUV              | 300 nm–400 nm                      | 3.10–4.13 eV          |
| Ultraviolet B or medium wave | UVB              | 280 nm–315 nm                      | 3.94–4.43 eV          |
| Middle   | MUV              | 200 nm–300 nm                      | 4.13–6.20 eV          |
| Ultraviolet C, short wave, or germicidal | UVC              | 100 nm–280 nm                      | 4.43–12.4 eV          |
| Far      | FUV              | 122 nm–200 nm                      | 6.20–10.2 eV          |

![http://www.inventoland.net/img/blog/sources1.png](http://www.inventoland.net/img/blog/sources1.png)

(drawings of the actual spectrum)


---


## Light Sources ##

![http://www.olympusmicro.com/primer/lightandcolor/images/lightsourcesfigure3.jpg](http://www.olympusmicro.com/primer/lightandcolor/images/lightsourcesfigure3.jpg)

## Typical DLP Projector Lamp Spectrum ##

![http://upload.wikimedia.org/wikipedia/en/thumb/9/94/Mercury_Vapour_Lamp_Spectrum.jpg/800px-Mercury_Vapour_Lamp_Spectrum.jpg](http://upload.wikimedia.org/wikipedia/en/thumb/9/94/Mercury_Vapour_Lamp_Spectrum.jpg/800px-Mercury_Vapour_Lamp_Spectrum.jpg)


## Doping Effects on Mercury Lamps ##

![http://lemoncurry.googlecode.com/files/mercurylamps02.png](http://lemoncurry.googlecode.com/files/mercurylamps02.png)

## LED Spectra ##

![http://lemoncurry.googlecode.com/files/led_spectra00.jpg](http://lemoncurry.googlecode.com/files/led_spectra00.jpg)

## Xenon Arc Lamp Spectra ##

![http://lemoncurry.googlecode.com/files/xenon-arc-spectra00.jpg](http://lemoncurry.googlecode.com/files/xenon-arc-spectra00.jpg)

(Graphs of the actual spectrum)


http://zeiss-campus.magnet.fsu.edu/articles/lightsources/mercuryarc.html


More info on light sources

http://s1137.photobucket.com/albums/n506/IdeaPDish/spectra/


**Lens UV Attenuation**

http://www.schott.com/advanced_optics/german/download/schott_tie-35_transmittance_october_2005_en.pdf

[Corning Eagle XG](http://www.delta-technologies.com/downloads/Eagle%20XG.pdf)

[Corning Eagle 2000](http://www.delta-technologies.com/downloads/Eagle%202000.pdf)

---


## Print Speeds ##

![http://lemoncurry.googlecode.com/files/printspeeds.jpg](http://lemoncurry.googlecode.com/files/printspeeds.jpg)

[Print Speed Calculator Download](http://lemoncurry.googlecode.com/files/printspeeds01.xls)

(actual spreadsheet calculator)


---


## Printer Materials ##

# BOM #

Here's a place to enter in your favorite components:

[BOM on KitBOM](http://kitbom.com/kitbom/lemon-curry)


**DLP Projector**

![http://lemoncurry.googlecode.com/files/dlp-engine00.jpg](http://lemoncurry.googlecode.com/files/dlp-engine00.jpg)

DLP Engine (actual DLP projector chassis, not rendered)

**DLP color wheel type with mercury vapor lamp**

There is a manufacturer that has a DLP projector chassis without the needless color wheel and with a 385nm LED light source. Models are available in native resolutions from 800 x 600, 1024 x 768 and 1920 x 1080. They also have them with high output mercury lamps with a spectra that reaches to 385nm. I'll post the links when we get the model numbers.

The higher the native resolution of the projector the higher the resolution the prints will be.

For example a DLP with a native resolution of SVGA 800 x 600 may be used to print and area of 80mm x 60mm at 0.1mm resolution with a Z resolution controlled by the slice thickness and stage at 0.01mm.

Another example is a DLP with a native resolution of XGA 1024 x 768 may be used to print and area of 102mm x 77mm at 0.1mm resolution with a Z resolution controlled by the slice thickness and stage at 0.025mm.

### DLP Projector Modifications ###

**Color Wheel**

The color wheels in the projectors are used to filter the light into Red, Green and Blue light and also filter out the 385nm UV. The color wheel needs to be removed or modified to allow the 385nm UV to pass through the projector if used with UV sensitive photopolymers. For some models the color wheels may be simply removed. Other models may have an encoder on the wheel and the wheel will just need the filters removed so that the encoder will still feedback its motion to the projectors controller.

If you're using visible spectrum cured photopolymers the the color wheels don't need to be removed. http://bucktownpolymers.com/polymer01.html Several chemistries are available in Cyan, Magenta, Yellow, Black and White.

http://upload.wikimedia.org/wikipedia/commons/4/45/DLP_Colorwheel_IMG_5508.JPG
Typical DLP Projector Color Wheel (actual hand, not mine, actual color wheel, not rendered)

[Single-Panel DLP Projection System Optics](http://focus.ti.com/pdfs/dlpdmd/Discoverydlpa002.pdf)

**Lens**

The typical range of focus may be too far a distance and beam spread for a printer. The distance between the DLP and optical engine may need to be positioned farther away from the light engine to focus the projector only a few inches away on the vat.

**Lamps**

[Philips Cinema Xenon Lamps](http://www.lighting.philips.com/pwc_li/main/subsites/special_lighting/assets/Cinema_brochure_Febr_2011.pdf)


---


**Vat**

UV clear bottom vat large enough to hold the photopolymers and the stage.

The vat that holds the photopolymer may be constructed out of anything that doesn't leak, for top down projection systems. Glass, polymers, metals etc.

For bottom up projection systems the vat needs to be optically clear at the wavelength of the photoinitiators in the polymer. Another quality of the materials chosen for the bottom of the vat is that they should not adhere well to the exposed and cured photopolymer. Glass, silicones, PTFE, polyolefins and highly crystalline polymers tend to work well.

Sylgard 184 on glass works very well for many. Another option is a PTFE film over glass.

The viscosity of the photopolymers may be varied greatly by controlling their temperature while printing. A heated vat is necessary for a low viscosity. Cartridge type heaters lend themselves well to this application, but anything that safely heats the polymers will do. A runaway heater safety circuit is recommended to avoid fire or overheating.

---


**Z-Axis Positioner**

The positioner may be fabricated from t-slot framing, leadscrew, bearings and blocks, stepper motor and stepper motor driver.

---


**Stage**

The stage may be fabricated from wood, plastic or metal with a glass, metal or ceramic target surface to build the prints.

---


**Stepper Motor Driver**

A4988 Stepper Motor Driver Carrier with Voltage Regulators
http://www.pololu.com/catalog/product/1183

or similar

---


**Machine Design**

Some websites and forums about machine design. Many might benefit from reading through discussions about well designed machines and the principles involved.

http://buildyourtools.com/phpBB3/

http://www.cnczone.com/

---


**USB IO Controller**

Teensy USB Board, Version 2.0
http://www.pjrc.com/store/teensy_pins.html

---


**Firmware**

Sprinter
https://github.com/kliment/Sprinter

---


**Software**

Skeinforge for Slicing
http://www.skeinforge.com

Slicer
http://slic3r.org/

Printrun
http://reprap.org/wiki/Printrun

Gary Hodgson much improved version of Printrun
https://github.com/garyhodgson/Printrun

---


**Photopolymers**

http://bucktownpolymers.com

Several chemistries are available in Cyan, Magenta, Yellow, Black and White
UV and UV through visible spectrum versions.


---


# [Please Post Your Comments & Questions Here](http://code.google.com/p/lemoncurry/wiki/Comments) #

We created a comments and questions page since the wiki front page was getting so long. All the comments and questions have been moved there.