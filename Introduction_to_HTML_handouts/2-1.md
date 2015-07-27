![](headers/head2.1.jpg)
# Introduction

In this lesson we are going to talk about what HTML is, what it is used for and its main concepts.

# HTML

HTML stands for **Hypertext Markup Language** so it's not a programming language, but rather a markup language. By definition **hypertext** is essentially text that has links to other texts. The linking capacity of the web is one of the main foundations of the Internet revolution. Web pages are basically text and media which have links to other pages, which in turn link to others and so on. The concept of having this web of links in a non-linear fashion is what is called hypertext.

The other term, **markup**, means that a standard kind of code – that is, HTML – is used to properly present text, links and other elements on the web page. HTML uses **tags** to mark the elements, and that's where the term markup comes from. HTML is used just to structure content and to reflect its meaning in form of code. For example, if we have some text that represents a title, we will mark it as a heading using a heading tag. If we have some text that represents a paragraph, we'll use a paragraph tag, and so on.

# What are tags?

Tags are special words between angled brackets. Most tags open and close, like these paragraph tags here:

```html
<p>This is a paragraph.</p>
```

The slash indicates the closing tag and the content goes between tags. For example, the content in this example is marked up as a paragraph.

We can also specify more information for the tag by using **attributes**. Attributes are extra information that we attach to the tag, like **id". In this example the "welcome" id is assigned to this paragraph:

```html
<p id="welcome">This is a paragraph.</p>
```

Ids can be used as hooks for HTML and for other languages like CSS and JavaScript.

There are other kinds of tags with which we only use attributes. They're called **void tags** because they contain no content and no closing tag, just attributes. For example

* `br` tag for line breaks
* the `meta` tag for information about the page
* `img` tag for images

You'll learn more about them in future lessons.

# More about HTML

HTML is currently in version 5, which has become a buzzword in recent years. The work of the WHATWG, or Web Hypertext Application Technology Working Group, along with the browser makers, the web community, and the World Wide Web Consortium (W3C), has culminated in this important evolution of the language, which it is still happening. After ten years of HTML being stagnant, we are seeing progress much more quickly and that opens a lot of possibilities for web professionals. In the future lessons you will learn more about HTML's history.

One other important advancement of the use of HTML was the Web Standards movement and the importance of separating front-end layers. When we use HTML, we are working with the front end of a page. Front-end languages, like HTML, CSS and JavaScript, are interpreted by the browser. Back-end languages, like PHP, run on the server's side. As we've seen, the role of HTML in front-end coding is to structure and define content. In the page it was common to use tags to make the text bold, have it a certain color, or even to control the page's layout. However we must not use HTML for presentational purposes, because this job is done with CSS. So with HTML we are only going to think about the base structure, and whether the tags we are using have the closest meaning to what we are trying to convey with the content - that's what semantic HTML is all about.

Now let's put all these concepts into practice. In the next lesson we are going to build a basic HTML page.