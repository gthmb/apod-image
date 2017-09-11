[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg?style=flat-square)](https://www.webcomponents.org/element/gthmb/apod-image)
# \<apod-image\>

A Polymer 2.0 Custom Element for displaying NASA's Astromony Picture of the Day

By default, the element will show today's APOD image. By setting the `date` attribute, you can select an image for a date in the past.

The default `apod-image` has an info toggle button that can be tapped to toggle an overlay containing the title, explanation and date of the image. This overlay, and the ability to toggle it via the toggle button, can be enabled/disabled by setting attributes on your `apod-image` instance. Please see the [api page](https://www.webcomponents.org/element/gthmb/apod-image/elements/apod-image) for the element's documentation.

If you want to use a custom information overlay, you can set the `custom-info` attribute on your instance. The markup you want to show for the overlay should be passed into the `info` slot. Please see the [demo page](https://www.webcomponents.org/element/gthmb/apod-image/demo/demo/index.html) for an example.

While most of the APOD images are actually images, sometimes NASA shares a YouTube video instead. In this case, the `apod-image` will render a YouTube player when the `apod-request` returns a video instead of an image.

Live Example (needs valid API Key to render):
<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="apod-image.html">
    </div>
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<!-- the tag -->
<apod-image api-key="my-nasa-api-key"></apod-image>
```
^ Replace `my-nasa-api-key` with a valid api key. Need One? [Get one here](https://api.nasa.gov/index.html#apply-for-an-api-key). See the demo for some working examples.