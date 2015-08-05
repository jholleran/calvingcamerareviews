---
layout: post
heading:  "Remoting Viewing"
subHeading:  "Internet Calving Camera System"
date:   2015-07-20 21:36:00
bg-img: internet-connected-bg.png
description: |
  How to connect and configure your calving camera system up to the Internet? There are two main way to accomplish with a static IP address from your ISP or with a DDNS. This article will describe in detail how to setup can configure both of these options.

categories: internet
---

How to connect and configure your calving camera system up to the Internet? There are two main way to accomplish with a static IP address from your ISP or with a DDNS. This article will describe in detail how to setup can configure both of these options.

#Static IP Address
The first option is to get a static IP address of your Internet Service Provider (ISP). Usually by default your ISP will not assign a static IP address to your Internet connection. The assigned address can change from time to time. The way it works is, when your modem is started and tries to connect to the Internet it requests an IP address from the ISP. The ISP will return an IP address which will be set on the modem. This address will be used to communicate with other computers on the Internet.

There will be a charge for a static IP address which could be 20 to 30 euros per year. Depending on your ISP it could be different. Once you get your static IP address you will need to set this on your modem. Check the user manual of your modem it see how to set this up.

Here how to do set this on an Eircom D1000 Modem:

- Go to Network Settings page
- Click Broadband tab
- Find Internet Connection section
- Look for IP Address label
- Enter Static IP Address provided by your ISP

Once this is set up you will be able to connect to your Modem from anywhere in the world. Simply type the IP address into a Web Browser. This should display the login page of your Modem. 


Next step is to set a static IP address on the IP camera that is unique from within the Local Area Network (LAN). This is not the same IP address that was provided by the ISP. All network devices from within your LAN can be configured with a static IP address that you control. This is to make sure that accessing the camera is always through the same IP. Also, make sure you set the same Subnet Mask that is set on your modem.

For example this is an example ip camera settings: 

- IP Address: 192.168.1.8
- Subnet Mask: 255.255.255.0
- Port: 8080

##Port Forwarding
The next step is to allow the IP camera to be accessed through the modem. The modem will need to be configured to open the port that the camera is running on. Traffic connecting to that port is forwarded on to the camera. This process is called Port Forwarding.


Here are the usual way to set this but your modem may differ:

- Go to Network Address Translation (NAT) page
- Open Port Forwarding tab
- Click Add New Rule button
- Enter the IP address of the camera and the port number. 


You should now be able to connect to your camera by entering the static ip address followed by the port number:
&lt;static ip&gt;:&lt;port&gt;. 
For example if your ip address is 78.37.21.192 and the camera is running on port 8080 then enter 78.37.21.192:8080 into a Web Browser. This should display the camera console web page. From there you can view the video from the camera.

If there is an issue at this point where it doesn't display anything. This could be blocked by the Firewall on the Modem. You might need to open the port on the firewall to let traffic through.


{% include break.html %}

#DDNS
The second option to connecting a calving camera system up to the Internet is to use a Dynamic Domain Name Service ([DDNS](https://en.wikipedia.org/wiki/Dynamic_DNS) or DynDNS). This service works by assigning a domain name to the IP address of your local network. The DDNS will then forword all requests make to this domain name to the IP address.
As the IP address of the local network will change from time to time the DDNS will need told about. A DDNS client will need to be running on the local network. This will inform the DDNS service of any changes so it can keep its domain name index up to date.

##Domain Names
A domain name is an easier name to remember than an IP address. An example of this is: http://mycamera.dydns.org. This can be typed directly in a browser. This will goto the DDNS which will forward the request to the IP address of the network. 


##Setting up a DDNS Account
There are many different compainies on the Internet that provide DDNS services. One of them is DynDNS where you can set up a account. If you want a custom domain name, for example; http://myfarmcalvingcamera.com you will need to pay a small fee for this.

Its very simple to set this up. Go to a DDNS provider and open an account. You will be able to create a domain name that will be easily remembered.

##DDNS Client
The next thing that needs to be setup is the DDNS client. This is a small software program that periododicly polls the IP address assigned to the local network. If it discovers that it has changed then it connects to the DDNS service and informs it of the new IP address. The DDNS service takes this new IP address and updates its domain name index. Now when someone enters your domain name into a browser the DDNS will forward this request to the correct IP address.

When that is set up go to the camera and enter the DDNS information on the camera. Now everytime the IP address changes the camera will automatically connect to the DDNS and inform the service that the IP address has changed. The DDNS will now forward requests to the domain name to the new IP address.

##Modem with DDNS Client
Most modems have a DDNS client built in enternally. This allows the modem to inform the DDNS that the IP assigned to the local network has changed. This is very easy to setup. Go to device settings on the modem and look for DDNS settings. From there, you can enter the DDNS account information so it can access it to do the update. This will always be the best place to have a DDNS client running as the modem will be the first to know about IP address changes.

##Camera with DDNS Client
Some IP cameras also contain a DDNS client. This allows the camera to inform the DDNS that the IP of the local network has changed. This is very easy to setup on the camera. Go to device settings and look for DDNS settings. From there you can enter the DDNS account information so it can access it.


##PC with DDNS Client
If neither the modem or IP camera have a DDNS client built in a DDNS client can be installed on a PC. Your DDNS provider will have a DDNS client that can be downloaded. This will run the IP update. The only disadvantages to this is that the PC will need be running at all times to keep the DDNS updated.

