---
layout: post
title:  "What is that aircraft?"
date:   2023-09-10 21:26:00 -0600
categories: DSP SDR ADS-B virtual radar
permalink: /virtual-radar
excerpt: "What is that aircraft"
---
## Summary
The public can certainly use FlightAware, but what about that plane flying over right now? Answer, Virtual Radar (hardware + SDR + mapping software).

## Residential Locations
At several points, I have lived in fairly close proximity to departure or arrival paths of local airports. Several times, I had wondered 'what is that aircraft and where is it going?'

## Craft Locations
It has taken some time for public industry adoption/requirement, but many aircraft are now equipped with Automatic Dependent Surveillance - Broadcast (ADS-B) beacons.

## Setup/Requirements
There are a fair number of instructions available out there, but the basics required are:
* An SDR receiver hardware (USB + antenna)
* An SDR program to tune and use DSP to decode the incoming signals
* It is useful to have a mapping program to plot the location and paths of the various beacons received.

## Results
A virtual RADAR system that will plot the position and information of all the beacons the setup can effectively receive.

## Additional Considerations
* Military/Government craft may not have transponders turned on for various reasons
* The homebrew setup may not be able to pick up every single craft for various propagation reasons
* There was a demonstration at a BlackHat conference several years back that spoofed an ADS-B transponder
    * This could be exploited as a DDoS-style "attack" if remote ATC relied primarily on ADS-B beacons for information.
        * ATC has other methods of RADAR for cross-checking RADAR readings.
