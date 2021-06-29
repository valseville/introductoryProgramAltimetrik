# HTML 
## What is XHTML?
- XHTML stands for EXtensible HyperText Markup Language
- XHTML is a stricter, more XML-based version of HTML
- XHTML is HTML defined as an XML application
- XHTML is supported by all major browsers

**Why this is called XHTML?**
XML is a markup language where all documents must be marked up correctly (be "well-formed").
XHTML was developed to make HTML more extensible and flexible to work with other data formats (such as XML). In addition, browsers ignore errors in HTML pages and try to display the website even if it has some errors in the markup. So XHTML comes with a much stricter error handling.
This is the old version of HTML and has major differences compared to HTML5.

**The Most Important Differences from HTML**
- <!DOCTYPE> is mandatory
- The xmlns attribute in <html> is mandatory
- <html>, <head>, <title>, and <body> are mandatory
- Elements must always be properly nested
- Elements must always be closed
- Elements must always be in lowercase
- Attribute names must always be in lowercase
- Attribute values must always be quoted
- Attribute minimization is forbidden

**What is HTML?**

The HTML acronym stands for Hyper Text Markup Language, so it’s a markup language, not a programming language. But what does this even mean? What is a Markup language?

In computer text processing, a **markup language** is a system for annotating a document in a way that is visually distinguishable from the content. It is used only to format the text so that when the document is processed for display, the markup language does not appear.

The way how to HTML distinguish the content is with the called HTML Tags

E.g. ```<h1> <h2> <p> <a>```

These tags describe a specific type of content like headings, paragraphs, or links. The tags mark up the begging and the end of an element

E.g. ```<tagname>content</tagname>```


**Meta tags**

The ```<meta>``` tag defines metadata about an HTML document. Metadata is data (information) about data.
```<meta>``` tags always go inside the ```<head>``` element and are typically used to specify a character set, page description, keywords, author of the document, and viewport settings.
Metadata will not be displayed on the page but is machine parsable.
Metadata is used by browsers (how to display content or reload the page), search engines (keywords), and other web services.
There is a method to let web designers take control over the viewport (the user's visible area of a web page), through the ```<meta>``` tag
E.g.
```<head>```
 ``` <meta charset="UTF-8">```
 ``` <meta name="description" content="Free Web tutorials">```
 ``` <meta name="keywords" content="HTML, CSS, JavaScript">```
  ```<meta name="author" content="John Doe">```
  ```<meta name="viewport" content="width=device-width, initial-scale=1.0">```
```</head>```

**Open Graph meta tags**
Are snippets of code that control how URLs are displayed when shared on social media. 
They’re part of Facebook’s Open Graph protocol and are also used by other social media sites, including LinkedIn and Twitter (if Twitter Cards are absent).
You can find them in the ```<head>``` section of a webpage. Any tags with ```og:``` before a property name are Open Graph tags.
og:title - The title of your object as it should appear within the graph, e.g., "The Rock".
og:type - The type of your object, e.g., "video.movie". Depending on the type you specify, other properties may also be required.
og:image - An image URL that should represent your object within the graph.
og:url - The canonical URL of your object that will be used as its permanent ID in the graph, e.g., "https://www.imdb.com/title/tt0117500/".
Usage e.g.
```<meta property="og:title" content="How to Become an SEO Expert (8 Steps)" />```
```<meta property="og:description" content="Get from SEO newbie to SEO pro in 8 simple steps." />```
```<meta property="og:image" content="https://ahrefs.com/blog/wp-content/uploads/2019/12/fb-how-to-become-an-seo-expert.png" />```

**Input Types in HTML**
Input is put (data) into a computer, for this, we have a different types depending on what information the web or app requires. The most common input types are: 
```<input type="button">```
```<input type="checkbox">```
```<input type="color">```
```<input type="date">```
```<input type="email">```
```<input type="file">```
```<input type="image">```
```<input type="month">```
```<input type="number">```
```<input type="password">```
```<input type="search">```
```<input type="submit">```
```<input type="tel">```
```<input type="text">```

## Links
- https://www.udemy.com/course/design-and-develop-a-killer-website-with-html5-and-css3/
- https://ahrefs.com/blog/open-graph-meta-tags/
- https://ogp.me/
- https://www.w3schools.com/html/html_form_input_types.asp
- https://www.w3schools.com/tags/tag_meta.asp
- https://www.w3schools.com/html/html_xhtml.asp
- https://www.w3schools.com/xml/xml_usedfor.asp
- https://es.wikipedia.org/wiki/XHTML
- https://www.youtube.com/watch?v=bLfrc_Nv_pY