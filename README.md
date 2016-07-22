# Infinite Carousel

Showcasing recent projects or high profile clients is essential to attracting new customers. [Solodev's](https://www.solodev.com/) infinite carousel cycles through dozens of items with contemporary styling and necessary responsiveness. Using [Slick Slider by Ken Wheeler](http://kenwheeler.github.io/slick/), this carousel can be adapted to fit your website needs and add a touch of agency inspired design.


## Tutorial

For detailed instructions, view Solodev's [Adding an Infinite Client Logo Carousel to your Website](https://www.solodev.com/blog/web-design/code-examples/adding-an-infinite-customer-logo-carousel-to-your-website.stml) article.

## Demo

Check out a working example on [JSFiddle](https://jsfiddle.net/solodev/huten0wq/).

## HTML

The form includes basic HTML markup:
```
<section class="customer-logos slider">
	<div class="slide"><img src="images/image1.png"></div>
	<div class="slide"><img src="images/image2.png"></div>
	<div class="slide"><img src="images/image3.png"></div>
	<div class="slide"><img src="images/image4.png"></div>
	<div class="slide"><img src="images/image5.png"></div>
	<div class="slide"><img src="images/image6.png"></div>
	<div class="slide"><img src="images/image7.png"></div>
	<div class="slide"><img src="images/image8.png"></div>
</section>
```

## CSS

All CSS is included in carousel.css.

## JavaScript

In addition to the slick.js resource, the infinite carousel itself needs to be initialized with the following script:
```
<script type="text/javascript">
	$(document).ready(function(){
		$('.customer-logos').slick({
			slidesToShow: 6,
			slidesToScroll: 1,
			autoplay: true,
			autoplaySpeed: 1000,
			arrows: false,
			dots: false,
				pauseOnHover: false,
				responsive: [{
				breakpoint: 768,
				settings: {
					slidesToShow: 4
				}
			}, {
				breakpoint: 520,
				settings: {
					slidesToShow: 3
				}
			}]
		});
	});
</script>
```

For a full list attributes you can use to customize your carousel, visit [Slick Slider by Ken Wheeler](http://kenwheeler.github.io/slick/).

## External Includes

The form includes the following third-party resources:
```
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css" rel="stylesheet" type="text/css"/>
	
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js" type="text/javascript"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js" type="text/javascript"></script>
```