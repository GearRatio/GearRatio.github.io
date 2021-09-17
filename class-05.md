# Duckett HTML & CSS Chapters 5, 11, 12

-TL;DR

![Mr. Bean](https://media.giphy.com/media/Wv2BOzWTfqH8A/giphy.gif?cid=ecf05e47lx3c8cwdp3qbxzt8tfs3z97q2l5x5cm1tjrrrwjh&rid=giphy.gif&ct=g)

# Images
Images provide a message to websites. Below are some resources to help find that extra bit of pizzazz.
  * istockphoto.com
  * unsplash.com
  * Adobe Stock

Images should convey information, enhance the mood, fit the color palette. When you plan to include images on your page you should have a separate folder for them. File organization is highly recommended. This helps to be able to easily find the files needed to work on or update.

In order to add images you you the `<img>` tag. The tag also requires teh `src` `alt` and `title`. Save images in the correct format. Most popular are PNG, JPEG, and GIF.  PNG is a lossless compression so use this format for the sharpest images. JPEG has lossy compression and are best suited for photographs and paintings of natural scenes. Read - [JPEG vs PNG vs GIF](https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d)

The larger the image format the better the image will render on screens and smaller devices. Make sure when selecting an image you take into account a larger format that what you intend to use it for. When resizing images make sure you do so using pixels and nothing else. This helps to preserve the quality of the image when reducing its size.

## Color
You can specify colors in CSS using rgb, hex, and hue saturation and lightness, or (hsl). [Why CSS HSL Colors are Better!](https://elad.medium.com/why-css-hsl-colors-are-better-83b1e0b6eead)

Pay attention to foreground and background colors. Text needs to be high contrast in order for it to be readable. 

There are many sites to help with picking color pallets and generating hex codes along with HSL values. A quick google search can help you pull up many options.

## Text
Fonts are an important part of web design. They help set the mood and overall tone of the site. There are many styles and weights to choose from. Google fonts is an excellent resource to help select fonts and even provides you with links to include in your HTML files and default information for your CSS file.

Text size is handled by three values, pixels, percentages and EMS. An EM is equivalent to the width of the letter m.

You can specify a font using `@font-face` and including it within your CSS file. This is helpful is a user does not have the specific font loaded onto their computer.

```css
@font-face {
  font-family: "Font family goes here";
  src: url('');
}

```
The line-height property helps with line spacing. The property sets the height of the entire line or text. The larger the property the larger the line gap, many designers would refer to this aspect as leading. Letter-spacing adjusts the kerning of the letters and word-space adjusts the gap between each word.

Lastly, you can use pseudo-classes to change text, links, and elements when a user hovers over them. You can even specify how to style links by using `:link` or `:visited`.


## Area of focus for me
Over the weekend I plan to work on my lab form this week and focus on CSS and design. My hope is to create a more please page that is easy to read and conveys a few unique traits that are unique to me.



