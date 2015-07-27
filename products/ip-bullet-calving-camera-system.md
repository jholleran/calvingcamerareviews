---
layout: product
slug: ip-bullet-camera
title: IP Bullet Calving Camera System
subTitle: Calving Camera System with IP Bullet Cameras
image: ip-bullet-calving-camera-system.png
price: €820.00
rating: 4.1
description: This IP Calving Camera System comprises of bullet cameras, for high resolution, crisp and clear video, and directional antennas for long range Wi-Fi connectivity. This system is ideal when there is a long distance between the shed and the house.

images:
   - title: Hikvision IP Bullet Camera
     name: hikvision-ip-bullet-camera.png
   - title: Directional Antennas for long range Wi-Fi connectivity
     name: two-directional-antennas.jpg
   - title: Ethernet cabled to connect the equipement together
     name: 20-ethernet-cable.jpg
   - title: POE network switch for powering the antenna and cameras
     name: 8-port-poe-switch.png
   - title: POE Injector for powering the antenna (house side)
     name: poe-injector.png
   - title: Router to connect the system to PC or Laptop
     name: router.jpg
---

This Calving Camera System comprises of IP bullet cameras, for high resolution, crisp and clear video, and directional antennas for long range Wi-Fi connectivity. This system is ideal when there is a long distance between the shed and the house.

If you want to get more information about how to set this type of system see the following articles: 

 - [Bullet Cameras]({{site.baseurl}}/cameras/2015/07/12/bullet-cameras.html)
 - [IP Wireless Directional Antennas]({{site.baseurl}}/wireless/2015/05/26/ip-wireless-directional-antenns.html)



###Connection Diagram
Bellow is a connection diagram how the system is setup and connected together.

<figure>
  <img src="{{site.baseurl}}/img/connection-diagrams/bullet-ip-camera-antenna-connection-diagram.png" alt="IP Calving Camera System with Bullet Cameras">
  <figcaption style="text-align: center;">IP Calving Camera System with Bullet Cameras</figcaption>
</figure>
<br>

Here we have two IP bullet cameras connected to, and powered by, a POE network switch using ethernet cables. The POE network switch also connects, and powers, a directional antenna. 

The POE network switch simpifies the system by powering the cameras and the antenna through the ethernet cables. Without it, the other devices will need a separate power sources. If the system, you intend to build, will only ever have one camera then there is no need for the POE network switch, the camera can be connected directly to the antenna with an ethernet cable.

The directional antenna will make a Wi-Fi connection to the other directional antenna. These antennas will need a clear line of sight to maximise there range and connection quality. The maximum range of this is system 5km.

The directional antenna, at the house or office, is powered by POE injector and is connected to a router with ethernet cables. From there, a Laptop or PC can connect to the router which will all it to connect to the IP cameras and view the video remotely.

If the distance between the house and the shed is not that long, for example less than 100 meters, then the directional antenna can be left out of this system and connect the router to the POE network switch, on the shed side, with a direct ethernet cable.

This system can be easily expanded. To add more cameras just plug them into the POE network switch. As long as there are spare ports on the POE network switch then more cameras can be added. So, if you might need more cameras in the future its a good idea to have plenty of spare POE ports on the network switch.

###Equipment

- 2 IP Bullet Camera(s)
- 2 Wireless Directional Antennas
- 1 Four port POE Network Switch
- 1 POE Injector
- 3 20 meter Ethernet Cables
- 1 Router



<div class="pull-right">
  <b>Buy Now:</b>
  <button id="buy-{{ page.slug }}" data-product-title="{{ page.title }}" role="button" data-toggle="modal" class="btn btn-primary btn-large buy"><i class="icon-shopping-cart icon-white"></i>{{ page.price }}</button>
</div>
<br/>