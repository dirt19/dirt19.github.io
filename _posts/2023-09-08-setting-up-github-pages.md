---
layout: post
title:  "Setting Up GitHub Pages with Jekyll"
date:   2023-09-08 08:25:00 -0600
categories: jekyll update github
permalink: /setup
excerpt: "I recently set up a GitHub Pages blog with Jekyll. Here are some thoughts."
---
The instructions are everywhere and seem fairly straightforward when reading them. However, software changes. Instructions get outdated, dependencies get updated, and compatibility breaks. That is part of the reason that IT, computer, and software folks have jobs.

Some local machine specifications:
  * OS: Windows 10, build 19045.3324
    * AMD A10-8700P Radeon R6
    * 12.0 GB RAM
    * 1TB HDD (ST1000LM024 HN-M101MBB)
  * Windows Subsystem for Linux (WSL) version: 1.2.5.0
  * WSL OS: Ubuntu 20.04.1 LTS (kernel 4.4.0-19041-Microsoft)
  * Ruby version: 2.7.0p0
  * jekyll version: 3.9.3

While deploying this site, I ran into some issues.
  1. The system ruby version was not compatible with the most recent version of Jekyll. So, I installed a downlevel version of Jekyll that was compatible with the GitHub Pages dependencies.
  1. I tried using several themes and theme packs. The GitHub Pages would not deploy with some of the themes that worked just fine locally. Even ones that indicated compatibility. So, I have not bothered with additional themes for the moment.
