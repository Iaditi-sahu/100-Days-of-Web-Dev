# Responsive Images
** The problem is, images have inherent dimensions. We can’t stretch a photo that’s 500×250 pixels to anything beyond 500 pixels wide because it’ll get pixelate. Retina displays and mobile devices complicate things even more. To make our images responsive, we now have to take three things into consideration:

    The device’s dimensions
    The image’s dimensions
    The device’s screen resolution
This will be more difficult than media queries, which were only concerned with device width. But don’t worry, there are standard ways to solve all these problems, and we’ll walk you through them one step at a time.

* Retina Screens
**Retina screens have twice as many pixels per inch than standard-resolution screens. That is to say, each retina pixel is the equivalent of 4 standard pixels. This has a big impact on how images are displayed in a web browser.To render correctly on a retina device, an image needs to be twice as big as its final display dimensions.

* Responsive SVG Images
