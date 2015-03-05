![](headers/head3.5.jpg)
# Introduction

In this lesson we are going to overview some complementary text tags that can be useful in a variety of situations. To prepare for the lesson you may either open up the *"othertags-finish.html"* file that has all the completed examples or the *"othertags-begin.html"* if you wish to play with the tags yourself.

The tags that we are going to discuss are a little less used than the others that were covered so far, but it's important that you know what they are for to use them should the need arise.

# Q, blockquote and cite tags

The first group of tags is related to quotation.

We have the `q` tag used for inline quotations:

```html
<p>
	According to the <cite><a href="http://www.w3.org">W3C</a></cite> The q tag <q cite="http://www.w3.org/TR/html-markup/q.html">represents some phrasing content quoted from another source</q>.
</p>
```

We can also use the `cite` attribute to provide a link to the source.

Remember, that all tag appearances are styled using the default styles of the browser. You must not use the tag because it looks this or that way – a tag must be used to semantically mark up a piece of content. The style can then be changed with CSS.

# Blockquote tag

Next, we have the `blockquote` tag for long quotations:

```html
<blockquote>
	<p>
		Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quam, vero, quibusdam, odio fugiat eum corrupti ea id consequuntur enim in tenetur recusandae minus earum doloribus eos dolore molestias! Corrupti, saepe.
	</p>
</blockquote>
```

This tag can contain other tags like paragraphs, the `footer` tag, or the `cite` tag.

Next there is the `abbr` tag for abbreviations and acronyms:

```html
<p>
	<abbr title="Hypertext Markup Language">HTML</abbr> - abbr tag, for abbreviations and acronyms.
</p>
```

We can use the `title` attribute to explain what the abbreviation or acronym stands for. By default a tooltip will pop up showing the contents of the attribute when user places the cursor over the acronym.

# The time tag

The `time` tag for a brief while was removed from the specification only to be added again. It can be used to mark up a machine readable date, time or duration. That can be done using the `datetime` attribute:

```html
<p>
	<time datetime="2014-12-01 10:00:00">12/01/2014</time> - time tag
</p>
```

The next two tags are used a lot with code samples. The first one is the `code` tag used to mark up computer code:

```html
<p>
	<code>code tag</code>, for code
</p>
```

The other one is the `pre` tag for preformatted text in which structure is represented by typographic conventions rather than by elements:

```html
<pre>
Pre tag for preformatted text, like code samples
	<code>
		&lt;html&gt;
			&lt;head&gt;
				&lt;meta charset="UTF-8"&gt;
				&lt;title&gt;Title&lt;/title&gt;
			&lt;/head&gt;
			&lt;body&gt;
			
			&lt;/body&gt;
		&lt;/html&gt;
	</code>
</pre>
```

The `pre` tag respects the whitespaces inside it unlike the rest of the HTML code. It's very useful for presenting code samples with proper indentation and spacing. Just don't forget to put the code tag inside the `pre` tag if you are writing code inside it. The `&lt;` and `&gt;` represent the less than and greater than symbols and are called **HTML entities**. We are going to take a closer look at them in a later lesson.

# The span tag

Another tag we haven't covered yet is the `span` tag. This tag is a generic inline element used mainly as a hook for CSS.

```html
<p>	
	<span>span tag</span> - generic tag for use as CSS hook
</p>
```

Use this tag if you just want to style an inline element with CSS without attaching any particular meaning to the content.

The sister tag to it is the very commonly used `div` tag, the generic block level tag that we're going to analyse later.

A new tag in HTML5, the `mark` tag is used to highlight text within a context:

```html
<p>
	<mark>mark tag</mark> - highlight text within a context
</p>
```

An example would be when a search engine is highlighting the text within a link that matches what you have typed.

# The HR tag

The `hr` tag presents a level break. It shouldn't be used to separate sections of the page but rather to separate topics between paragraphs of text:

```html
<hr>
```

By default it is being rendered as a horizontal line.

# Former presentational tags revised for HTML5

There are some formerly presentational tags from HTML4 and earlier that had their meaning changed in the HTML5 specification. Let's go over some of them.

The `small` tag was used to render smaller text. But this is CSS' job so now it is being used to mark up less important information on a website like copyright or legal notes.

```html
<p>
	<small>small tag</small> - formerly used to render small text, semantics modified in HTML5. Now used for the &ldquo;small print&rdquo; of websites.
</p>
```

The `b` and `i` tags that previously made the text bold or italic respectively also had their meaning updated.

```html
<p>
	<b>b tag</b> - former bold tag, semantics modified in HTML5. Used to highlight text without any extra importance. <a href="http://www.w3.org/html/wg/drafts/html/master/text-level-semantics.html#the-b-element">more information here</a>.
</p>

<p>
	<i>i tag</i> - former italic tag, semantics modified in HTML5. Similar to <code>b</code>, used to mark up text in an alternate voice or mood. <a href="http://www.w3.org/html/wg/drafts/html/master/text-level-semantics.html#the-i-element">more information here</a>.
</p>
```

The `b` tag can be used to highlight text without conveying any extra importance. It should be used as a last resort, and only when there's no other better option available.

The `i` tag represents text in an alternative voice or mood like taxonomic designations or technical terms.

Other tags include `s`, `u`, `del`, and `ins`.

```html
<p>
	<s>s tag</s> - former strike-through tag, semantics modified in HTML5. Now used for content that is no longer relevant.
</p>

<p>
	<u>u tag</u> - former underline tag, semantics modified in HTML5. Can be used to represent <q>text with an unarticulated, though explicitly rendered, non-textual annotation, such as labeling the text as being a proper name in Chinese text (a Chinese proper name mark), or labeling the text as being misspelt</q> (W3C). <a href="http://www.w3.org/html/wg/drafts/html/master/text-level-semantics.html#the-u-element">more information here</a>. The default appearance of the tag can confuse the user because it looks like a link, so this tag should be used with caution.
</p>

<p>
	<del>del tag</del> - deleted content from the document.
</p>

<p>
	<ins>ins tag</ins> - added content in the document.
</p>
```

The `s` tag is now used for text that is no longer relevant.

The `u` tag, the former underline tag, can be used now for texts that represents an unarticulated though explicitly rendered non-textual annotation, such as labeling the text as being a proper name in Chinese text, or labeling the text as being misspelt. As you see these are very specific use cases, and the default appearance of the tag can confuse the user because it looks like a link. So, if you are going to use u tag, use it with caution.

The `del` and `ins` tags represent deleted and added contents of the documents respectively.
