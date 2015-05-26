---
layout: post
heading:  "IP Directional Antennas"
subHeading:  "IP Wireless Directional Antennas"
date:   2015-05-26 22:40:00
bg-img: calving-camera-creevagh.jpg
description: |
  Building a Calving Camera System with a IP Directional Antenna for long distances between the Shed and the House. This article describes how to set Directional Antennaa up and how to integrate them with IP Cameras.

categories: wireless
---

#Directional Antennas
IP Directional Antennas contain both a transmitter and a receiver. This means there is a two way communication between the two IP Directional Antennas. Two way communication is important if you wish to use a <a href="/ptz/2015/04/26/ptz-calving-camera.html">PTZ IP Camera</a> and control the viewing angle for the camera remotely.

Directional Antennas transmit radio waves in a single direction. The signal will only be picked up the direction that its pointing. As it focuses the radio waves in one direction it can transmit and receive longer distances than Omi-directional Antennas. In most farms, this is exactly what is needed for setting up a Calving Camera as the Shed can be a long distance from the House.

##Set Up
IP Directional Antennas are very simple to connect together. On one side, the IP Camera plugs directly into one of the Directional IP Antenna with a Ethernet cable. One the other, the second Directional Antenna plugs directly in a Router, PC, or Laptop with another Ethernet Cable. When the antennas are set up to communicate with one another you will be able to connect to the camera from your PC or Laptop.

##Ubiquiti NanoStation
The <a href="http://www.amazon.com/gp/product/B004EGI3CI/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=B004EGI3CI&linkCode=as2&tag=jhollerano-20&linkId=APRWR6VNXX5WNQRM">Ubiquiti NanoStation loco M2</a><img src="http://ir-na.amazon-adsystem.com/e/ir?t=jhollerano-20&l=as2&o=1&a=B004EGI3CI" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" /> is a very good, plug and play, product that is very simple to integrate with most IP Cameras, and other network devices. 

The loco M2 transmits at 150 Mbps, which is very fast and is more than enough to transmit live video from the Camera very smoothly. It also has a very long range of 5+ km, which is sufficient for most farms, but if you need a longer range you can get the <a href="http://www.amazon.com/gp/product/B004EHSV4W/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=B004EHSV4W&linkCode=as2&tag=jhollerano-20&linkId=D2ICM7EKQFEM2PIO">Ubiquiti NanoStation loco M5</a><img src="http://ir-na.amazon-adsystem.com/e/ir?t=jhollerano-20&l=as2&o=1&a=B004EHSV4W" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" /> which will transmit up to 10+ km.

These Antennas can be used outdoors and can be mounted to a pole.

##POE
These Directional Antennas are power by <a href="http://en.wikipedia.org/wiki/Power_over_Ethernet">POE</a>. POE standes for Power Over Ethernet. This basically means that the Antenna is powered by the Ethernet Cable and means that there is no need for a separate power cable.


##Wireless Security
Always make sure that the Wireless Security settings (WEP or WPA & WPA2) are set up correctly on these Antennas, and are password protected. This will encrypt the data being sent, to and from the antenna, and prevent other, unwanted guests, from hacking into your network. These radio signal from these Directional Antenna can picked up from a very long distance away so it would be better to be safe.


##Ubiquiti NanoStation loco M2
These antenna can be purchased on Amazon and are reasonably priced. Here is a link to one of them:

<iframe style="width:120px;height:240px;" marginwidth="0" marginheight="0" scrolling="no" frameborder="0" src="//ws-na.amazon-adsystem.com/widgets/q?ServiceVersion=20070822&OneJS=1&Operation=GetAdHtml&MarketPlace=US&source=ac&ref=qf_sp_asin_til&ad_type=product_link&tracking_id=jhollerano-20&marketplace=amazon&region=US&placement=B004EGI3CI&asins=B004EGI3CI&linkId=NACNL6576ZSEOJ4Y&show_border=true&link_opens_in_new_window=true&price_color=BF3E3E&title_color=759BBD&bg_color=F9F3F3" />

