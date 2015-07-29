---
layout: post
heading:  "Remoting Viewing"
subHeading:  "Connecting a Calving Camera System up to the Internet"
date:   2015-07-20 21:36:00
bg-img: three-cows-in-shed.jpg
description: |
  How to connect and configure your calving camera system up to the Internet? There are two main way to accomplish with a static IP address from your ISP or with a DDNS. This article will describe in detail how to do this.

categories: internet
---

#Static IP Address
The first option is to get a static IP address of yor Internet Service Provider (ISP). 

An IP address is in the following format xxx.xxx.xxx.xxx

Usually by default your ISP will not assign a static IP address for you. The IP address that is assigned to you can change from time to time. The way it works is, when your modem is started and tries to connect to the Internet it requests an IP address from the ISP. The ISP will return an IP address which will be set on the modem. This address will be used to communicate with the Internet.

For two computers to talk to one another, over the Internet, they both need a unique IP address. The reason for this is that data been send from one machine needs to contain an address of the machine it wants to send the data to so that the network can route it to that machine. This is a lot like putting an address of a person on a letter.

Every device that is communicating with the Internet needs an IP address. The problem with IP address numbers is that there is not enough unique addresses available for every device in the world. To get around this problem ISP's have a pool of IP addresses that assigns out to network devices when they need to want an Internet connection for a period of time. When the device is finished with the IP address is goes back into the address pool so it can be assigned to a different device.

Wide Area Network (WAN)
Local Area Network (LAN)
IP Address: 192.168.1.254
Subnet Mask: 255.255.255.0



If you want your Local Area Network (LAN) to have its own unique static IP address then you can request this from your ISP. Call them up and ask for a static IP address for your Internet connection. There will be a charge for this which could be 20 to 30 euros per year. But depending on your ISP it could be different. 
Once you get your static IP address you will need to set this on your modem. Each router settings page will be different so check your user manual about how to do this.

Here how to do set this on an Eircom D1000 Modem:
Network Settings
Broadband
Internet Connection
IP Address label
Set Static IP Adress and enter the IP provided by your ISP

Once this is set up you will be able to connect to your Modem by entering the IP Address in a browser from anywhere in the world.
The next step is to allow the IP Camera to be accessed through the modem. The modem will need to be configured to open the port that the camera is running on and forward traffic connecting to that port to the camera. This is called Port Forwarding.

IP Camera: 
192.168.1.8
Port: 8080


Network Address Translation (NAT)
Port Forwarding
Add New Rule
Enter the IP address of the camera and the port number. You should now be able to connect to your camera by entering the static ip address followed by the port number:
So for example: 78.37.21.192:8080

This should now display the camera console web page there you can view the video from the camera.

If there is an issue at this point where it doesn't display anything. This could be blocked by the Firewall on the Modem. You might need to open the port on the firewall to let it through.



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

