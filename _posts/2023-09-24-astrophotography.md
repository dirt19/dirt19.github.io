---
layout: post
title:  "DSLR Milkyway Photography"
date:   2023-09-24 19:25:00 -0600
categories: DSLR astrophotography optics calculations
permalink: /dslr-astro
excerpt: "The Milkyway is beautiful this time of year."
---
## Summary
I wanted to calculate the maximum exposure time for a stationary (untracked) photo shoot with a DSLR (Digital single-lens reflex) camera. There are several elements to take into account in the calculations: sensor size, sensitivity, crop factor, focal length, speed of apparent celestial rotation depending on area of sky (field rotation), etc.

## Equipment
* Camera: Canon EOS Rebel T5
* Lens: 18-55mm (f/3.5 - 5.6)
* Tripod
* External lens trigger

## Broad to Specific
There are many sites that mention "The Rule of 500" as being a good enough solution for amateurs and standard photography kit. The rule says to take 500 and divide it by the focal length of the lens to get the maximum number of seconds for exposure before stars start to trail. Taking a "kit" Canon lens (18-55mm), 500/18 gives 27.7 sec before stars start trailing. This may get us in the vicinity, but is still too long.

This calculation seems to have come about during film photography and was based on the size of silver grains on the particular type of film that was used. It can be used to get an idea of the range of the times that would result from making more detailed calculations. With the development of smaller digital sensors in DSLR cameras, the Rule of 500 evolved into the Rule of 300. The smaller sensors made with smaller pixels meant the tolerance in smudging was reduced, so the stars appeared to make trails faster. Taking the same lens and focal length 300/18 gives 16.6 sec before stars start trailing. However, this may still be too long.

The question becomes, "how much sky does one pixel cover?" and "how do I minimize star trails?" The answer is complicated by several additioanl factors: the view of the area of sky,  how much that part of the sky will move with respect to the observer, the size of the stars (may be more than one pixel), the sensitivity of the sensors, how noisy the sensors are, quality of the lens (chromatic aberations from the lens, etc), whether the moon or other bright objects are in the sky:
* Example Sensor:
    * Sensor Size: 22.3 x 14.9 mm
    * Pixels: 5184 x 3456
    * Pixel size: 4.3um
    * crop factor: 1.61
    * ISO (sensor sensitivity)
    * T: tolerance assume visible smudge at 5px
    * sensor noise
* Example Lens:
    * fl: focal length
* Example Observer location:
    * lat: 40 N
    * lon: 105 W
    * Earth Rotational Speed (degrees per second)
* Field of View / Area of sky
    * Declination

## Post Photoshoot Processing
* After capturing the desired images, "black frames" can also be taken so that the noise can be subtracted from the captured frames.

## Short Version
"There isn't a short version, but somewhere between 9 and 25 seconds is a good range to experiment with."

## References
* [Lonely Speck - Advanced Astrophotography Shutter Time Calculator](https://www.lonelyspeck.com/advanced-astrophotography-shutter-time-calculator/)
* [Kelly Flanagan - Field Rotation and Alt-Azimuth Mounted Telescopes](https://kelly.flanagan.io/astronomy/astrophotography/field-rotation-and-alt-azimuth-mounted-telescopes/)
* Dark Sky calculators
* Photo processing software
