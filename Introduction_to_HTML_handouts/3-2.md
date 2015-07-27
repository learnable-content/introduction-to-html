![](headers/head3.2.jpg)
# Introduction

In this lesson you are going to learn how to include images in a document. To prepare for the lesson open up the file named *"images-begin.html"* provided in the lesson files. It already has the basic HTML structure within the body tag. Also note the *"picture.jpg"* file in the same folder.

Images are added to web pages using a tag called image, or `img`. It's a void element, so as you remember it does not have a closing tag and we work only with its attributes. Let's try it:

```html
<img>
```

However currently this tag does basically nothing. We have to specify the path to the file that should be displayed on the web page. To do that use the source attribute – `src`. Our file is in the same folder as the HTML document, so we can just write its name:

```html
<img src="picture.jpg">
```

Now reload the document in the browser and note that the image is already being shown.
The images added can have different formats like GIF, JPEG, and PNG.

# Width and height attributes

It's also possible to specify the image's width and height with the help of corresponding attributes, though that's better done with CSS. The sample image's size is 400 by 400 pixels, so we can specify that:

```html
<img src="picture.jpg" width="400" height="400">
```

Notice that we just wrote the number without a unit. Another unit we can use with this attribute is the percent unit:

```html
<img src="picture.jpg" width="100%" height="100%">
```

Now the browser will stretch the image to 100% width and height of the page, however that won't look nice. So if you want to keep the image from distorting, it is better to provide only one of the dimensions and let the browser figure out the rest.

```html
<img src="picture.jpg" width="600">
```

In most cases `width` and `height` attributes are not necessary, so you may remove them.

# The alt attribute

The `alt` attribute presents an alternative text to the user when the image cannot be loaded, or if the device accessing the page cannot show images: for example, screen readers – kind of browser used by people with blindness or visual impairments – or search robots like the Google bot, which indexes the Internet by visiting web pages. Such kind of software only sees the page's code so this is the reason to have clear and semantic HTML code: it will help users and search engines to better understand the page's content.

So we should use the `alt` attribute to provide alternative content for the image:

```html
<img src="picture.jpg" alt="Tree with pink blossoms">
```

It is a good practice to include `alt` attribute in every image tag. In cases when you don't have text to insert into the `alt` attribute, use an empty string. However if you can't think of a good descriptive text for the alt attribute, chances are that the image is only decorative and should be included via CSS.

# Other media tags

There are also other advanced tags we can use to insert media. We'll take a very brief look at them as they are subjects for another course.

* `video` tag that allows to insert video in the web page
* `audio` tag allows to insert audio files
* `embed` and object tags are used to insert various types of files, mainly SWF (Flash) files
* `picture` tag is currently a draft specification that is going to make life easier for designers and web developers. It's a like an `img` tag but with many more features. This element was introduced following the need for creating an `img` tag that works well with responsive websites, which have to adapt to multiple screen sizes and pixel densities.