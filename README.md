# Carousel (No JS)

Carousel made using Jade and Stylus.

Free use.

Pre-made version can be found in `carousel.min.css`, it assumes 550&times;500px size.

---

Inspired by <https://www.reddit.com/r/web_design/comments/4k8x5d/image_carousel_css_only_no_js_required/>

# Example code:

`````jade
include carousel-mixin

- var tafttest = "https://tafttest.com/"
- var x = "x"
- var png = ".png"
- var carouselcont = [tafttest+800+x+600+png, tafttest+600+x+800+png, tafttest+800+x+800+png, tafttest+600+x+600+png, tafttest+500+x+800+png, tafttest+800+x+500+png, tafttest+500+x+500+png, tafttest+300+x+800+png, tafttest+800+x+300+png, tafttest+720+x+720+png]

+carousel(10, carouselcont)
`````

You need to know how many items there are in a carousel before you add it. If there's another way (amount in array) please tell me.

The CSS is easier, as it is Stylus based.

You can change it in the file by changing these variables:

`````stylus
$carouselWidth = 550px;
$carouselHeight = 500px;
$carouselSpinnerWidth = 50px;
$carouselSpinnerFontSize = 62px;
$carouselRadius = 4px;
$carouselDotTopMargin = ($carouselHeight/10)*9.5;
$carouselMargin = 30px;

$carouselFullScreenSize = 27px;
$carouselFullScreenSizeFS = $carouselFullScreenSize*2;
`````

They are moderately self-explanatory and are only needed to change a small amount. For the most part though changing is not required.

It's just as fast as a JS-based version but without the mixture of compatibility. It is almost guaranteed to work and can change more often.

View live demo: <https://dizzyzane.github.io/carousel-css/>
