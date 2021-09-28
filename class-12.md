# Intro to Chart.js and Canvas

Chart JS is a plugin that allows developers to easily construct pie charts, line graphs, bar charts, and more. Because this is my first time using it and reading out it. I am going to try and walk through the set up and usage of Chart.js.

There are a few ways you can being using Chart.js. I believe the most common was is to include a link from Chart.js, `<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>`. Although, it also appears you can install using npm. I am unclear which option is best but believe importing the script is the most likely approach.

1. In order to begin to use the script you need to use the `<canvas>` tag and include an `id`. You can set the  width and height of the chart in-line and are optional per MDN docs. Without specifics the default values will be 300 pixels by 150 pixels. You can also use CSS to control the width and height.

2. When no styling is provided the chart will be fully transparent.

3. It is a good idea to provide fallback content when for older browsers with limited support. Only older browsers will recognize the fallback content. [Example](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)


    ```html
  <canvas id="clock" width="150" height="150">
    <img src="images/clock.png" width="150" height="150" alt=""/>
  </canvas>
    ```

4. In order for the Canvas element to render it's content you need to be sure to use the `getContext()` method. It takes one parameter and for this example it will be `2D`.

5. You can also use canvas to draw shapes using a `function draw()`. This can be used to create shapes, draw paths, triangles. There are some important methods that can be used in conjunction such as `moveTo(x, y)`. There are many more uses within.

6. Once shapes are drawn you can also use `fillStyle` or `strokeStyle` to help with applying colors to shapes. `globalAlpha` allows you to draw semi-transparent or translucent shapes. There are many options to implement in order to create a unique appearance if desired.

7. Similar to drawing shapes you also have the ability to draw text using two methods. `fillText` and `strokeText`.

In summary, Chart.js is a powerful tool that has a ton of flexibility. As I learn more about it today I will provide an update on specific instillation and use for implementing a chart on my project.


[Back to TOC](README.md)

