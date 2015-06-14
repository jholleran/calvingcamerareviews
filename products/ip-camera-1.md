---
layout: product
id: ip-camera-1
title: IP Camera
subTitle: PTZ Calving Camera
image: IP-PTZ-CAM-1.jpg
price: 78
rating: 4
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
				<span id="rating-{{ page.id }}" data-rating="4.2" data-star-big="Yes" class="stars" title="good" style="cursor: default; width: 100px;">
					<img src="/img/star-on-big.png" alt="1" title="good">&nbsp;
					<img src="/img/star-on-big.png" alt="2" title="good">&nbsp;
					<img src="/img/star-on-big.png" alt="3" title="good">&nbsp;
					<img src="/img/star-on-big.png" alt="4" title="good">&nbsp;
					<img src="/img/star-off-big.png" alt="5" title="good">
					<input type="hidden" name="score" value="{{page.rating}}" readonly="readonly">
				</span>
				<span>{{page.rating}}</span>
			</p>
		</div>
	</div>
</div>

<h3>Product Summary</h3>
<div>Network IP Camera with Pan, Tilt &amp; Zoom.</div>