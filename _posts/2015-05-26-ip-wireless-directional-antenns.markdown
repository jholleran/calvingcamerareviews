---
layout: post
heading:  "Directional Antennas"
subHeading:  "IP Wireless Directional Antennas"
date:   2015-05-26 22:40:00
bg-img: ip-directional-antennas-bg.png
text-color: gray
nav-color: gray
description: |
  IP Directional Antennas can be used when there is a long distance between the Shed and the House. This article describes how to set a directional antenna up and how to integrate them with IP Cameras.

categories: wireless
---

<h2>Directional Antennas</h2>
IP Directional Antennas contain both a transmitter and a receiver. This means there is a two way communication between the two IP Directional Antennas. Two way communication is important if you wish to use a <a href="/ptz/2015/04/26/ptz-calving-camera.html">PTZ IP Camera</a> and control the viewing angle for the camera remotely.

Directional Antennas transmit radio waves in a single direction. The signal will only be picked up the direction that it's pointing. As it focuses the radio waves in one direction it can transmit and receive longer distances than Omi-directional Antennas. In most farms, this is exactly what is needed for setting up a Calving Camera as the Shed can be a long distance from the House.

<h2>Set Up</h2>

<figure>
  <img src="{{site.baseurl}}/img/connecting-buildings-colored.png" alt="Connecting buildings with Directional Antennas" style="width: 100%;">
  <figcaption style="text-align: center;">Connecting buildings with Directional Antennas</figcaption>
</figure>

IP Directional Antennas are very simple to connect together. On one side, the IP Camera plugs directly into one of the Directional IP Antenna with an Ethernet cable. One the other, the second Directional Antenna plugs directly in a Router, PC, or Laptop with another Ethernet Cable. When the antennas are set up to communicate with one another you will be able to connect to the camera from your PC or Laptop.

Here is a connection diagram of how the Direction Antennas are integrated into the Calving Camera System.


<figure>
  <img src="{{site.baseurl}}/img/ip-camera-antenna-connection-diagram.png" alt="IP Calving Camera System with Directional Antennas">
  <figcaption style="text-align: center;">IP Calving Camera System with Directional Antennas</figcaption>
</figure>
<br>

<h2>Ubiquiti NanoStation</h2>
The <a href="https://www.ubnt.com/airmax/nanostationm/">Ubiquiti NanoStation loco M2</a> is a very good, plug and play, directional antenna that is very simple to integrate with most IP Cameras, and other network devices. 

The loco M2 transmits at 150 Mbps, which is very fast and is more than enough to transmit live video from the Camera very smoothly. It also has a very long range of 5+ km, which is sufficient for most farms, but if you need a longer range you can get the Ubiquiti NanoStation loco M5 which will transmit up to 10+ km.

These Antennas are suitable to be used outdoors and can be mounted to a pole or chimnely.
For more information about these antennas see the <a href="https://www.ubnt.com/airmax/nanostationm/">Ubiquiti NanoStation Web Site</a>.

<h2>POE</h2>
These Directional Antennas are power by <a href="http://en.wikipedia.org/wiki/Power_over_Ethernet">POE</a>. POE stands for Power over Ethernet. This basically means that the Antenna is powered by the Ethernet Cable and means that there is no need for a separate power cable.


<h2>Wireless Security</h2>
Always make sure that the Wireless Security settings (WEP or WPA & WPA2) are set up correctly on these Antennas, and are password protected. This will encrypt the data being sent, to and from the antennas, and prevent other, unwanted guests, from hacking into your network. The radio signal from these Directional Antenna can picked up from a very long distance away so it would be better to be safe.

<h2>Buy On Amazon</h2>

<iframe style="width:120px;height:240px;" marginwidth="0" marginheight="0" scrolling="no" frameborder="0" src="//ws-eu.amazon-adsystem.com/widgets/q?ServiceVersion=20070822&OneJS=1&Operation=GetAdHtml&MarketPlace=GB&source=ss&ref=ss_til&ad_type=product_link&tracking_id=calvingcamera-21&marketplace=amazon&region=GB&placement=B004ZCKNYW&asins=B004ZCKNYW&linkId=&show_border=true&link_opens_in_new_window=true">
</iframe>



<div>
<br>
<div class="fb-like" data-href="{{ page.url | prepend: site.url }}" data-layout="standard" data-action="like" data-show-faces="true" data-share="true"></div>
</div>


{% assign page = site.data.long-range-cc-system-data %}
{% include product-preview.html %}
