---
# layout: post
title:  "DSLR Milkyway Photography"
date:   2023-09-13 10:25:00 -0600
categories: DSLR astrophotography optics calculations
excerpt: "The Milkyway is beautiful this time of year."
---
## Summary
I wanted to calculate the maximum exposure time for a stationary (untracked) photo shoot with a DSLR (Digital single-lens reflex) camera. There are several elements to take into account in the calculations: sensor size, sensitivity, crop factor, focal length, speed of apparent celestial rotation depending on area of sky (field rotation), etc.

## Equipment
* Camera: Canon EOS Rebel T5
* Lens: 18-55mm (f/3.5 – 5.6)
* Tripod
* External lens trigger

## The short and fast version
There are many sites that mention “The Rule of 500” as being a good enough solution for amateurs and standard photography kit. The rule says to take 500 and divide it by the focal length of the lens to get the maximum number of seconds for exposure before stars start to trail. Taking a “kit” Canon lens (18-55mm), 500/18 gives 27.7 sec before stars start trailing. This may get us in the vicinity, but is still too long.

This calculation seems to have come about during film photography and was based on the size of silver grains on the particular type of film that was used. It can be used to get an idea of the range of the times that would result from making more detailed calculations. With the development of smaller digital sensors in DSLR cameras, the Rule of 500 evolved into the Rule of 300. The smaller sensors made with smaller pixels meant the tolerance in smudging was reduced, so the stars appeared to make trails faster. Taking the same lens and focal length 300/18 gives 16.6 sec before stars start trailing. However, this may still be too long.

The question becomes, “how much sky does one pixel cover?” and “how do I minimize star trails?”

## Elements of Consideration
* Sensor:
    * Sensor Size: 22.3 x 14.9 mm
    * Pixels: 5184 x 3456
    * Pixel size: 4.3um
    * crop factor: 1.61
    * ISO (sensor sensitivity)
    * T: tolerance assume visible smudge at 5px
    * sensor noise
* Lens:
    * fl: focal length
* Observer location:
    * lat: 40 N
    * lon: 105 W
    * Earth Rotational Speed (degrees per second)
* Field of View / Area of sky
    * Declination

## References


