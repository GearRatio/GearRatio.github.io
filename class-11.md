# Images and Practical Information

## Images
It is important to understand how to control images when laying out a site. Images very in size and due to the high contrast they may take longer to load than other parts of the page. By controlling images, or standardizing them, it is possible for the images to load faster resulting in less delays.

The book recommends using the width and height of the images and assigning classes to them in order to properly classify them when using in the / selecting them. By identifying the images up front you can then implement them where needed on your site.

The book also recommends using float to help allow text to flow around images. Images are inline elements and in order for text to flow around them. The author suggested to use classes in order to help ID the photos needed to help text flow around them.

Centering images can be achieved using text-align or by using margin-left, margin-right, and setting both to auto. Also, when centering an image it is important to turn the image into a `block` element.

The book also discusses the use of background-images. The can be repeated, positioned, and layered. The shorthand for background-image is `background`. The properties must be used in order. An example has been provided below.

```html
body{
background: color, url(), repeat, position;
}
```
A **sprite** is a single image that is used for several different parts of an interface. Examples would be a logo, interface elements, and buttons.

CSS3 allows the use and creation of gradients. These can be used as background colors. They are created using the background-image property. However, there are many resources on the web to help auto generate gradients.

If using a background image it is important to control the contrast of the image. Especially if you want to overlay text on it. Additionally, can you can reduce the opacity of the image if needed or create a blur effect on the text box that is on top of the image.

## Practical Information

Search Engine Optimization is a huge part of having a successful website. It is important to pay attention to some basic things that can help improve SEO. There are on-page techniques and off-page techniques. On-page techniques consist of ensuring keywords are used in your HTML. This helps search engines find your site and pull up in the results list. Search engines rely heavily on the text that is included in your pages so it is important to pay attention to what is being included. There seven key places to help you optimize SEO on-page.
  1. Page Title
  2. URL/Web Address
  3. Headings
  4. Text
  5. Link Text
  6. Image Alt Text
  7. Page Descriptions

Off-page SEO consists of linking to other sites. This helps search engines to ID relevant information between the two sites. The more relevant the better the SEO. Example, if you owned a bicycle shop your site would link to other bicycle manufacturers, lines that you carry. It wouldn't link to things that interest the shop owner or don't relate to bicycles.

There are ways to help organize an approach to SEO optimization. The book describes a process on pages 481 through 482. Google also offers tools to help measure and improve SEO. See Google's Search Console. Google also offers analytics that help track visitors, unique visits, and time spent on a page. You can sign up at google.com/analytics. It provides you a tracking code that you need to embed in your `<head>` tag and just before the `</head>` tag.

Lastly, when placing a site on the web it is a good idea to have a custom domain name and consider using a web hosting company. Many things come with these service provides and can help streamline the process of launching a site.

[Back to TOC](README.md)