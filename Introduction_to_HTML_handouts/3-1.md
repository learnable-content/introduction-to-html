![](headers/head3.1.jpg)
# Introduction

In this lesson we will review the main HTML tags used to mark up text. To prepare for this lesson open up the file *texttags-begin.html* provided in the lesson files. This file is already using the basic structure we have defined in the previous lesson. Also, there is some content in the body ready to be tagged. Open this file in the browser as well.

You as a web developer will have to identify and mark up content correctly. Of course there may be several ways of tagging a specific piece of content, but the most important recommendation is to try and apply tags that are coherent with their role of each part of the content in the document.

Before we start, let me pinpoint one thing. When you open the file in the browser, you'll notice that the text appears in one continuous line, while in the document there are line breaks and empty lines present. This is because HTML does not consider more than one space between texts so keep that in mind.

# H1 and p tags

The first line in the body is the main heading of the page. **Headings** represent any kind of titles you may have for sections of your page. HTML let us define six levels of heading: from one to six. This should be used in a hierarchy, so a heading level one would be the main title of a section or a whole page. The heading level two, in turn, should be put below it in hierarchy and used as a subtitle.

To define headings we use the tags `h1` to `h6`.

```html
<h1>HTML</h1>
```

The browser applies default styles to the headings. If you save the file and reload the page, you'll see that the heading is now bold and has bigger font size. The size of the heading will vary according to the number on the tag. Please note that you should not use these tags just to change the text size, or to make the font bold as this is CSS' job. In HTML we must not think of the visual presentation of the page but rather to analyse and see if the tags that we are using are helping to reflect the meaning of the page's content.

Next, we have two paragraphs of text. They will be marked up with the paragraph tag `p`:

```html
<p>HTML or HyperText Markup Language is the standard markup language used to create Web pages.</p>

<p>HTML is written in the form of HTML elements consisting of tags enclosed in angle brackets (like &lt;html&gt;). HTML tags most commonly come in pairs like &lt;h1&gt; and &lt;/h1&gt;, although some tags represent empty elements and so are unpaired, for example &lt;img&gt;. The first tag in a pair is the start tag, and the second tag is the end tag (they are also called opening tags and closing tags).</p>
```

You can now reload the page in the browser to check that the text is separated into two blocks.

# Strong and em tags

In the first paragraph the "HyperText Markup Language" is an important piece of information so we have to mark it somehow. When we have to set apart some important text, we can use the `strong` tag for strong emphasis:

```html
<p>HTML or <strong>HyperText Markup Language</strong> is the standard markup language used to create Web pages.</p>
```

By default browser will make text bold, however this can be changed easily with CSS.

When we want to emphasize a part of the text, we can use the `em` tag:

```html
<p>HTML or <strong>HyperText Markup Language</strong> is the standard markup language used to create <em>Web pages</em>.</p>
```

The default appearance for this tag is italic text, but remember that the emphasis meaning here is more important then the visual aspect.

# More heading tags

The next titles in out document are below in hierarchy, so we should follow a sequence in the headings. For example, "History" is a subtitle of the main title "HTML", so an `h2` tag is suitable here:

```html
<h2>History</h2>
```

"Development" is a subtitle of "History", so, here we should use an `h3`:

```html
<h2>History</h2>
<h3>Development</h3>
```

Then we have a paragraph:

```html
<h2>History</h2>
<h3>Development</h3>
<p>[...]</p>
```

And then another subtitle of the "History" section, so use `h3` again:

```html
<h2>History</h2>
<h3>Development</h3>
<p>[...]</p>
<h3>HTML versions timeline</h3>
```

"November 24, 1995" is a subtitle of "HTML versions timeline" so tag this as `h4`:

```html
<h2>History</h2>
<h3>Development</h3>
<p>[...]</p>
<h3>HTML versions timeline</h3>
<h4>November 24, 1995</h4>
```

Then another paragraph:

```html
<h2>History</h2>
<h3>Development</h3>
<p>[...]</p>
<h3>HTML versions timeline</h3>
<h4>November 24, 1995</h4>
<p>[...]</p>
```

And lastly other subtitles:

```html
<h2>History</h2>
<h3>Development</h3>
<p>[...]</p>
<h3>HTML versions timeline</h3>
<h4>November 24, 1995</h4>
<p>[...]</p>
<h5>heading level 5</h5>
<h6>heading level 6</h6>
```

You can now check how this looks in the browser so far.

# BR tag

For the address in the bottom of the document we are going to use a paragraph again:

```html
<p>Example Address
City, Country</p>
```

However in this example we need to force a line break. This can be done with the `br` tag:

```html
<p>Example Address
<br>
City, Country</p>
```

Reload the page and note how the text breaks, and starts again in the next line. The `br` tag is a void element, so it does not have a closing tag.