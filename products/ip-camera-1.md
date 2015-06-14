---
layout: product
id: ip-camera-1
title: IP Camera
subTitle: PTZ Calving Camera
image: IP-PTZ-CAM-1.jpg
price: 78
rating: 2.6
text-color: gray
---

<div class="hero-unit">
	<div class="row">
		<div class="col-md-3">
			<img src="/img/products/{{ page.image }}" id="tooltip-ip-camera-1" rel="tooltip" title="Preview" class="img-polaroid small-img" />
		</div>
		<div class="col-md-7">
			<p>
				<strong>Title:</strong>
				<span>{{page.title}}</span>
				<br>
				<strong>Price:</strong>
				<span>{{page.price}}</span>
				<br>
				<strong>Rating:&nbsp;</strong>
				<span class="stars" id="rating-{{ page.slug }}" data-rating="{{page.rating}}" data-suspended="suspended" data-star-big="Yes">
				</span>
				<span>{{page.rating}}</span>
			</p>
		</div>
	</div>
</div>

<h3>Product Summary</h3>
<div>Network IP Camera with Pan, Tilt &amp; Zoom.</div>