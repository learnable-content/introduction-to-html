![](headers/head3.3.jpg)
# Introduction

In this lesson we are going to learn how to create **lists** with HTML. To prepare for this lesson open up the file named *"lists-begin.html"* provided in the lesson files.

Lists are primarily used to format text, but in general they can be used to mark up anything you want, for example, a list of images in an image gallery or a list of links to create a navigational menu. 

There are two main kinds of lists that we can use: **unordered** and **ordered** lists. Ordered lists are those in which items are numbered. In all other cases unordered lists, where items are not numbered, are used.

# Let's start with an unordered list

Let's start with an unordered list. To define an unordered list employ the `ul` tag and inside it put the items in `li` tags which stands for list items:

```html
<ul>
	<li>4 main sections</li>
	<li>1 contact form</li>
	<li>Made with HTML, CSS and JavaScript</li>
</ul>
```

This is an example of a simple unordered list. You may now check how it's rendered in the browser.

# ol tag

For the ordered list, the idea is the same. Employ the `ol` tag and then insert the `li` inside:

```html
<ol>
	<li>Briefing</li>
	<li>Planning</li>
	<li>Design</li>
	<li>Development</li>
	<li>Publication</li>
</ol>
```

In fact lists can contain much more than just text so let's look at another example.

# Nested lists

Let's create an unordered list with a nested list inside it:

```html
<ul>
	<li>Home</li>
	<li>
	Products
	<ul>
		<li>Books</li>
		<li>Games</li>
	</ul>
	</li>
	<li>Services</li>
	<li>Contact Us</li>
</ul>
```

We can create sublists in any `li` just by creating another list inside the list item. Now save the file and check the result.

# A simple navigation menu markup

To sum up let's see an example illustrating the common use of lists: navigational menus. Most websites' menus are made with lists and then transformed with CSS. The mark up is going to be very simple:

```html
<ul>
	<li>Home</li>
	<li>Products</li>
	<li>Services</li>
	<li>Contact Us</li>
</ul>
```

Then, let's add another tag around the text – the **anchor** tag that is used to mark up links. We're going to learn more about this tag in the next lesson.

```html
<ul>
	<li><a href="#">Home</a></li>
	<li><a href="#">Products</a></li>
	<li><a href="#">Services</a></li>
	<li><a href="#">Contact Us</a></li>
</ul>
```

We've created a basic mark up for a website's menu. Check that in your browser.

Lists are very versatile and can be used in many different scenarios: not only to format texts or links, but also to mark up products, photos in a photo gallery, and much more.