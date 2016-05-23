# No JavaScript Carousel, using a Jade mixin

Carousel made using Jade and Stylus.

Free use.

## Installation

```
npm install jade-carousel
```

## Usage

See the example in the `dist` folder.

In your jade file simply call the mixin, passing in an array of image objects and an optional name (ID) for the carousel.

```
-
  var carouselItems= [
    {altText: "myImage", url: "https://tafttest.com/800x600.png"},
    {altText: "myImage", url: "https://tafttest.com/600x800.png"},
    {altText: "myImage", url: "https://tafttest.com/800x600.png"},
    {altText: "myImage", url: "https://tafttest.com/800x800.png"},
    {altText: "myImage", url: "https://tafttest.com/600x600.png"},
    {altText: "myImage", url: "https://tafttest.com/500x600.png"},
    {altText: "myImage", url: "https://tafttest.com/800x500.png"},
    {altText: "myImage", url: "https://tafttest.com/300x600.png"},
    {altText: "myImage", url: "https://tafttest.com/800x300.png"},
    {altText: "myImage", url: "https://tafttest.com/720x720.png"}
  ]

+carousel(carouselItems, "myCarousel")
+carousel(carouselItems)
```

The CSS is in the `dist` folder. You can modify it or use as is by `@import`ing it into your Stylus/Sass/Less files.


## Development

1. Install dependencies:

```
npm install
```

2. Compile the source code:

```
npm start
```