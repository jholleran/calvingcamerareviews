---
layout: post
heading:  "Directional Antennas"
subHeading:  "IP Wireless Directional Antennas"
date:   2015-05-26 22:40:00
bg-img: ip-directional-antennas-bg.png
text-color: gray
description: |
  IP Directional Antennas can be used when there is a long distance between the Shed and the House. This article describes how to set a Directional Antenna up and how to integrate them with IP Cameras.

categories: wireless
---

#Directional Antennas
IP Directional Antennas contain both a transmitter and a receiver. This means there is a two way communication between the two IP Directional Antennas. Two way communication is important if you wish to use a <a href="/ptz/2015/04/26/ptz-calving-camera.html">PTZ IP Camera</a> and control the viewing angle for the camera remotely.

Directional Antennas transmit radio waves in a single direction. The signal will only be picked up the direction that it's pointing. As it focuses the radio waves in one direction it can transmit and receive longer distances than Omi-directional Antennas. In most farms, this is exactly what is needed for setting up a Calving Camera as the Shed can be a long distance from the House.

##Set Up
IP Directional Antennas are very simple to connect together. On one side, the IP Camera plugs directly into one of the Directional IP Antenna with an Ethernet cable. One the other, the second Directional Antenna plugs directly in a Router, PC, or Laptop with another Ethernet Cable. When the antennas are set up to communicate with one another you will be able to connect to the camera from your PC or Laptop.

Here is a connection diagram of how the Direction Antennas are integrated into the Calving Camera System.


<figure>
  <img src="{{site.baseurl}}/img/ip-camera-antenna-connection-diagram.png" alt="IP Calving Camera System with Directional Antennas">
  <figcaption style="text-align: center;">IP Calving Camera System with Directional Antennas</figcaption>
</figure>
<br>

##Ubiquiti NanoStation
The <a href="http://www.amazon.com/gp/product/B004EGI3CI/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=B004EGI3CI&linkCode=as2&tag=jhollerano-20&linkId=APRWR6VNXX5WNQRM">Ubiquiti NanoStation loco M2</a><img src="http://ir-na.amazon-adsystem.com/e/ir?t=jhollerano-20&l=as2&o=1&a=B004EGI3CI" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" /> is a very good, plug and play, product that is very simple to integrate with most IP Cameras, and other network devices. 

The loco M2 transmits at 150 Mbps, which is very fast and is more than enough to transmit live video from the Camera very smoothly. It also has a very long range of 5+ km, which is sufficient for most farms, but if you need a longer range you can get the <a href="http://www.amazon.com/gp/product/B004EHSV4W/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=B004EHSV4W&linkCode=as2&tag=jhollerano-20&linkId=D2ICM7EKQFEM2PIO">Ubiquiti NanoStation loco M5</a><img src="http://ir-na.amazon-adsystem.com/e/ir?t=jhollerano-20&l=as2&o=1&a=B004EHSV4W" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" /> which will transmit up to 10+ km.

These Antennas can be used outdoors and can be mounted to a pole.

##POE
These Directional Antennas are power by <a href="http://en.wikipedia.org/wiki/Power_over_Ethernet">POE</a>. POE stands for Power over Ethernet. This basically means that the Antenna is powered by the Ethernet Cable and means that there is no need for a separate power cable.


##Wireless Security
Always make sure that the Wireless Security settings (WEP or WPA & WPA2) are set up correctly on these Antennas, and are password protected. This will encrypt the data being sent, to and from the antennas, and prevent other, unwanted guests, from hacking into your network. The radio signal from these Directional Antenna can picked up from a very long distance away so it would be better to be safe.


<br/>

<hr style="border-top: 1px solid #000;" />
<div class="row">
     <div class="col-md-3">
        <!-- product image-->
        <a href="/products/long-range-ip-calving-camera-system.html"><img src="/img/products/ip-calving-camera-system.png" class="img-polaroid small-img"></a>
     </div>
     <div class="col-md-8">
        <!-- product title--><a href="/products/long-range-ip-calving-camera-system.html"><strong>Long Range IP Calving Camera System</strong></a>
        <div>
           <!-- product rating-->
        	<span class="stars" id="rating-long-range-ip-camera" data-rating="4.6" data-suspended="suspended" data-star-big="Yes"></span>
			<span>4.6</span>
        </div>
        <!-- product information-->
        <br/>
        <div>
           <!-- buy button-->
        	<a href="/products/long-range-ip-calving-camera-system.html" id="buy-ip-camera-1" data-product-title="Wireless PTZ IP Camera" role="button" data-toggle="modal" class="btn btn-primary btn-mini buy"><i class="icon-shopping-cart icon-white"></i>€335.00</a>
        </div>
     </div>
     <script type="text/javascript" async="" src="http://www.google-analytics.com/ga.js"></script><script type="application/ld+json">
     {
        "@context": "http://schema.org",
        "@type": "Product",
        "name": "Long Range IP Calving Camera System",
        "offers": {
           "@type": "Offer",
           "price": "€335.00",
           "priceCurrency": "EUR"
        },
        "aggregateRating": {
           "@type": "AggregateRating",
           "ratingValue": "4.6",
           "reviewCount": ""
        }
     }
     </script>
</div>  
