---
layout: products
permalink: /products/
title: Calving Camera Products
slides:
   - title: Calving Cameras
     heading: Monitor your cows during calving season
     text: Keeping a good eye on the welfare of your animals.
     image: /img/cow-and-calf-creevagh.png
     thumb: /img/cow-and-calf-creevagh.png
   - title: Directional Antennas
     heading: Long Range Wireless Connection
     text: 
     link: /wireless/2015/05/26/ip-wireless-directional-antenns.html
     image: /img/long-range-cctv.png
     thumb: /img/long-range-cctv.png
   - title: Remote Viewing
     heading: Watch your cows in there pens from the comfort of your home.
     text: 
     image: /img/cows-in-pen.jpg
     thumb: /img/cows-in-pen.jpg
   - title: Mobile Devices
     heading: Combatible with most Mobile devices
     image: /img/major/s8.png
     thumb: /img/major/s8t.jpg
   - title: Internet
     heading: Connect System to the Internet
     image: /img/major/s2.png
     thumb: /img/major/s2t.jpg
---

<table class="table">
   <tbody>
   {% for page in site.pages %}
      {% if page.layout == 'product' %}
      <tr>
         <td class="col-md-2">
            <!-- product image-->
            <a href="{{ page.url }}"><img src="/img/products/{{ page.image }}" class="img-polaroid small-img"></a>
         </td>
         <td>
            <!-- product title--><a href="{{ page.url }}"><strong>{{ page.title }}</strong></a><!-- buy button--><button id="buy-ip-camera-1" data-product-title="Wireless PTZ IP Camera" role="button" data-toggle="modal" class="btn btn-primary btn-mini buy"><i class="icon-shopping-cart icon-white"></i>{{ page.price }}</button>
            <div>
               <!-- product rating-->
               <span class="stars" id="rating-{{ page.slug }}" data-rating="{{page.rating}}" data-suspended="suspended">
               </span>
                     <span>{{ page.rating }}</span>
            </div>
            <!-- product information-->
            <div>
               <small class="muted">
                  <div>{{page.catagory}}</div>
               </small>
            </div>
            <!-- product description-->
            <p>{{ page.description }}
            </p>
         </td>
      </tr>
      {% endif %}
   {% endfor %}
   </tbody>
</table>