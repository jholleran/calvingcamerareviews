---
layout: page
permalink: /products/
title: Products
subTitle: Calving Camera Products
bg-img: products_bg.png
description: |
  High quaility Calving Camera Systems available for purchase. Here you will find different types of systems to suit your needs, from IP PTZ Calvings to IP Bullet Cameras integrated with long range Directional Antennas.

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
            <!-- product title--><a href="{{ page.url }}"><strong>{{ page.title }}</strong></a>
            <!-- buy button-->
            <!--<button id="buy-ip-camera-1" data-product-title="Wireless PTZ IP Camera" role="button" data-toggle="modal" class="btn btn-primary btn-mini buy"><i class="icon-shopping-cart icon-white"></i>{{ page.price }}</button>
            -->
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
         <script type="application/ld+json">
         {
            "@context": "http://schema.org",
            "@type": "Product",
            "name": "{{page.title}}",
            "offers": {
               "@type": "Offer",
               "price": "{{page.price}}",
               "priceCurrency": "EUR"
            },
            "aggregateRating": {
               "@type": "AggregateRating",
               "ratingValue": "{{page.rating}}",
               "reviewCount": "{{page.reviews}}"
            }
         }
         </script>
      </tr>
      {% endif %}
   {% endfor %}
   </tbody>
</table>