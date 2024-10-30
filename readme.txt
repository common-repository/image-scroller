=== Image Scroller ===
Contributors: johnsmith48
Tags: flash, image, scroller, images, free, widget, css, effects, animation, text, html
Requires at least: 2.8.0
Tested up to: 3.1
Stable tag: trunk

Maybe the most advanced Image Scroller. Fully XML customizable without any Flash knowledge. And it's free!

== Description ==

The Image Scroller FX can be embedded in any website for free without even using Flash. It can have an overall width and height up to 1680 x 1050 pixels. It supports the following files: JPG, PNG, BMP, GIF for the thumbs, which are configurable through the images.xml file. The Scroller can be set to have infinite or finite scrolling, supporting different thumbs dimensions. There are a multiple highly customizable scroll properties like speed (on roll over or roll out), reflection, tooltip properties etc. On roll over can be applied different effects like: zooming, transparency, color saturation. An important thing is the low CPU usage for an extremely large number of thumbs. It has almost 60 configurable properties through a settings.xml file.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/image-scroller-fx.zip "Image Scroller FX Plugin") (that you have to install and activate) & [Free package](http://www.flashxml.net/free/download/image-scroller.zip "Image Scroller FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **image-scroller-fx** and copy the content of the **free package** there
3. If you copied the **free package** to a location different than the one above, go to **Image Scroller FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[image-scroller-fx][/image-scroller-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Image Scroller FX part of your theme, edit the template files and add `<?php imagescrollerfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Image Scroller FX](http://www.flashxml.net/image-scroller.html "Image Scroller FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/image-scroller-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/image-scroller-fx/images` and update the `wp-content/flashxml/image-scroller-fx/images.xml` file accordingly

= Additional settings file =

To embed the Image Scroller FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[image-scroller-fx settings="settings2.xml"][/image-scroller-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `imagescrollerfx_echo_embed_code()` function call (for example `<?php imagescrollerfx_echo_embed_code("settings2.xml"); ?>`).

= Add as widget =
To add the Image Scroller FX as a widget, go to **Widgets** from the **Appearance** tab in your *WordPress Dashboard*, then drag and drop the Image Scroller FX from **Available Widgets** to the widget area you want. You can specify a different `settings.xml` file and an alternative content for users without Adobe Flash Player from the widget's settings.

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[image-scroller-fx]` and `[/image-scroller-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `imagescrollerfx_echo_embed_code()` function call (for example `<?php imagescrollerfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[image-scroller-fx width="600" height="300"][/image-scroller-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `imagescrollerfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/image-scroller.html "Image Scroller FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/image-scroller-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/image-scroller.html "Image Scroller FX") is the utility that helps easily customize your Image Scroller FX to fit all your needs.