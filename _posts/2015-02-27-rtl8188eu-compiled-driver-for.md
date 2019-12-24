---
layout: post
title: RTL8188EU Compiled Driver for BeagleBone Black
date: '2015-02-27T12:38:00.002-08:00'
author: Christopher Kuzma
tags:
- TP-Link
- driver
- RTL8188EU
- TL
- black
- 8288eu.ko
- TL-WN723N
- WN723N
- beaglebone
- compiled
modified_time: '2015-04-12T17:50:59.821-07:00'
thumbnail: http://4.bp.blogspot.com/-6wNivkhKydI/VPDTKZauOaI/AAAAAAAAGsQ/yK8ekgvNrwk/s72-c/Screen%2BShot%2B2015-02-27%2Bat%2B15.26.26.png
---

<div class="separator" style="clear: both; text-align: center;"><a href="http://4.bp.blogspot.com/-6wNivkhKydI/VPDTKZauOaI/AAAAAAAAGsQ/yK8ekgvNrwk/s1600/Screen%2BShot%2B2015-02-27%2Bat%2B15.26.26.png" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="http://4.bp.blogspot.com/-6wNivkhKydI/VPDTKZauOaI/AAAAAAAAGsQ/yK8ekgvNrwk/s1600/Screen%2BShot%2B2015-02-27%2Bat%2B15.26.26.png" height="275" width="400" /></a></div><div class="separator" style="clear: both; text-align: left;"><br /></div><div class="separator" style="clear: both; text-align: left;">About a month ago <a href="http://blog.christopherkuzma.com/2015/02/beaglebone-black-my-personal-cloud.html" target="_blank">I picked up a BeagleBone Black</a> to use with my own projects. Shortly thereafter I snagged a free-after-rebate USB WiFi adapter from TigerDirect to use with it. I wasn't entirely sure whether or not I'd actually be able to use it with the BBB, but figured it was worth a shot given the price. What was the card in question? The diminutive TP-Link TL-WN723N.</div><div class="separator" style="clear: both; text-align: left;"><br /></div><div class="separator" style="clear: both; text-align: left;">Various guides on the internet exist that guide one through the process of installing the requisite kernel headers and missing system components in order to compile the driver for one's self. But what if you don't want to mess around with that? What if you're running the latest stock image of Debian on a BBB and simply want to install a precompiled driver and get going? That's what I've got to share with you here.</div><div class="separator" style="clear: both; text-align: left;"><br /></div><div class="separator" style="clear: both; text-align: left;">Because I found myself constantly making a mess of the base linux system, I decided to make a copy of my compiled driver so that I wouldn't have to recompile it every time I reflashed the eMMC. I figure it's probably useful for other people, too, so here it is. All instructions can be found on the GitHub page:</div><div class="separator" style="clear: both; text-align: left;"><br /></div><div class="separator" style="clear: both; text-align: center;"><b><a href="https://github.com/ckuzma/rtl8188eu-Driver-for-BeagleBone" target="_blank"><span style="font-size: large;">RTL8188EU Driver for the BeagleBone Black</span></a></b></div><div class="separator" style="clear: both; text-align: left;"><br /></div><div class="separator" style="clear: both; text-align: left;"><br /></div><div class="separator" style="clear: both; text-align: left;"><br /></div>