# Comments & Questions #

Comment by nomokie42, Mar 21, 2012

What are you using to drive the DLP? Seems to me it might be as efficient if not more to treat the design to be fabbed as a series of slices displayed via streaming video. Especially if the open-source version might typically use surplus/salvaged components.


---



Comment by PaulChainKang, Mar 22, 2012

Skeinforge, Printrun and your Sprinter are all based on G-codes which are for CNC type. With a DLP projector, it should project pictures of slicing but not direct G-code. How do you convert G-code to pictures?


---



Comment by Toby.Harcombe, Mar 23, 2012

Have you considered an LED DLP, but replace the LEDs with something like the Lumex Quaserbrite UV LED? They have them available in 385nm


---


Comment by project member A2ShedsJ, Mar 23, 2012

Each slice or layer is projected with the DLP for a small period of time, then the z-axis is moved for projection of the next layer.

The g-code is just used to move the z-axis, The images are vector 1-bit deep slices of the 3d models. Check the experimental branch of skeinforge and you'll see how it works.

Toby: Yes.



---


Comment by PaulChainKang, Mar 24, 2012


@A2ShedsJ,

Where can I get the experimental branch of skeinforge? Thanks in advance.
Delete comment
Comment by project member A2ShedsJ, Mar 24, 2012

The latest version should have what used to be in experimental: http://fabmetheus.crsndoo.com/files/50_reprap_python_beanshell.zip

IRC freenode #reprap or #lemoncurry for more info



---


Comment by PaulChainKang, Mar 24, 2012

@A2ShedsJ,

Thank you. I have some problems with the IRC freenode, can you point me out what directories/files I should look for slicing the model into vectored images? Appreciate your helps.

Paul Kang


---


Comment by nomokie42, Mar 26, 2012

Not to be questioning too much, but it seems like all you really need to rive the stepper is an accurate clock. (And possibly not a stepper.) I am wondering whether (once the optimal thickness and exposure time are worked out) all of this could be driven by something like a roku box with a usb stick in it.


---


Comment by Toby.Harcombe, Mar 26, 2012

Have you looked at using something like Makerslide for the Z axis?

---



Comment by project member A2ShedsJ, Mar 29, 2012

@ Toby sure it would work. Also wolf.arthur@gmail.com has http://www.contraptor.org/

Contrapteur is an open source construction set for grown-ups, based on a 20mm grid. It includes structural and mechanical components, and is a metric port of contraptor ( http://www.contraptor.org/ ). Release planned in april 2012. Ask arthur- about it and is also awesome

He will also have a LemonCurry? + contraptor design


---


Comment by lopsta.ecommerce, Apr 10 (4 days ago)

maker slider is a "linear bearing". usually those are quite expensive, but really only for higher length. this project will probably need around 20 cm for it, so the price shouldn't be such a big deal. it should be (in theory) more precise than maker slide so i think it's would be wise to use traditional linear bearings for this project. might be worth to buy for the sake of printing precision.


---


Comment by lopsta.ecommerce, Apr 10 (4 days ago)

contraptor is a replacement for t-slot profiles, not linear bearings. given the small size for this printer regular t-slots won't cost much. They are just a few dollar per meter.


---


Comment by Toby.Harcombe, Apr 11 (2 days ago)

Makerslide will be available at Inventables, it's pretty cheap at only $24.65 for 1200mm, but if you want higher precision, eBay is usually a great source for THK slides, and the short ones usually go cheap.


---


Comment by project member A2ShedsJ, Apr 11 (2 days ago)

@ lopsta http://www.contraptor.org/linear-rails-bearings-subset This subset includes linear rail pairs of different lengths from 6" to 24", as well as linear bearings.


---


Comment by primijos, Yesterday (31 hours ago)

Hi,

some questions about safety:

How safe is the material? (can it be touched without risk? accidental ingestion? can the build items be use to store food? does it produce any toxic vapors during the cure process?)

What about the light? Since it uses UV(A?) light, how does it compare to sun light exposure? I mean: can I use besides my laptop while doing other things without risk or must I keep myself away from the machine as long as possible (or, maybe, use sunscreen/aftersun? :-) )

(BTW, I have a 2 year old son and I would like to know how safe is the whole thing. Laser 3D printing is out of consideration completely, RepRap?/Makerbot/plastic\_extrusion\_in\_general seem to be OK, but looks far more complicated to build than Lemoncurry)

An idea/question about polychromatic printing: can the build material be "tweaked" to allow colour printing? Right now we're talking about a photosensible polymer that solidifies when the process is iniciated with some wavelength specific light, but... can it also be "excited" to get some specific color depending on some other parameters (for example: time exposure? Ideally "light color", but since you need to break the color wheel inside the projector I'm assuming there's no "color" in the light being projected)

By the way, very very nice work! Congratulations

Best, Jose


---


Comment by bbhessclh, Yesterday (17 hours ago)

Any recommendations for 1920 x 1080 resolution DLP projectors? Thanks!


---


Comment by elkn...@gmail.com, Apr 16 (6 days ago)

I'm considering doing something similar, but with an old laptop LCD panel like with this:

http://lifehacker.com/5479504/convert-your-old-laptop-into-a-digital-projector

and maybe a fresnel lens "Magna-Page" magnifier. Do you know of any reason why an LCD shutter and a plastic lens would not work? Will they pass sufficient UV?
Comment by kalle1...@gmail.com, Apr 16 (6 days ago)

I think this will not work with a color LCD panel. Every pixel is made with three colors (RGB), so the UV-wavelength will not go through red and green and also blue is bad i think. Maybe it works with an monochrome LCD, but there are no cheap highres available. I am very interested in your research, because i will make similar test in the next time. Perhaps it could be dome with a high power UV LED, but it seems to be not enough power.
Comment by wilb...@gmail.com, Yesterday (23 hours ago)

I am developing some simple software for making slices and coordinating the z-axis stepper control with projector exposure.

I am using: - Arduino USB serial interface - http://www.freesteel.co.uk/wpblog/slicer/ (for slicing .stl into .png) - Adobe AIR for exposure application (3DLP.exe)

I am looking for a git home for open sourcing it and yours looks like a good fit. If that is ok, could you add me as a member?


---


Comment by bruce.david.jones, Apr 26 (3 days ago)

I'm curious, what is the finest x/y resolution that can be achieved with this?
Delete comment
Comment by bobgarrish, Apr 27 (2 days ago)


---


It's entirely dependent on how small you focus your projector area.

If you have an 800x600 projector then you can print at 0.1mm accuracy over 80mm width or 0.01mm over an 8mm width. Seems insane to focus at 8mm, but the DLP chip is barely bigger than that so it's almost a direct shot.

1920x1080 projector can do ~0.005" (0.125mm) at a 10" (254mm) width. That's cooking with fire :)