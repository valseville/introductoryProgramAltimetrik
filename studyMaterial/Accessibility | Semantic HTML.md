# HTML Accessibility and Semantic
We call accessibility the concept of whether a product or service can be used by everyone.
As you learn more about HTML — read more resources, look at more examples, etc. — you'll keep seeing a common theme: the importance of using semantic HTML (sometimes called POSH, or Plain Old Semantic HTML). This means using the correct HTML elements for their intended purpose as much as possible.
You might wonder why this is so important. After all, you can use a combination of CSS and JavaScript to make just about any HTML element behave in whatever way you want. For example, a control button to play a video on your site could be marked up like this:
```<div>Play video</div>```

 

But as you'll see in greater detail later on, it makes sense to use the correct element for the job:
```<button>``` Play video``` </button>```


Not only do HTML ```<button>```s have some suitable styling applied by default (which you will probably want to override), they also have built-in keyboard accessibility — users can navigate between buttons using the Tab key and activate their selection using Return or Enter.

A semantic element clearly describes its meaning to both the browser and the developer. Semantic HTML doesn't take any longer to write than non-semantic (bad) markup if you do it consistently from the start of your project. Even better, semantic markup has other benefits beyond accessibility:

- **Easier to develop with** — as mentioned above, you get some functionality for free, plus it is arguably easier to understand.
- **Better on mobile** — semantic HTML is arguably lighter in file size than non-semantic spaghetti code, and easier to make responsive.
- **Good for SEO** — search engines give more importance to keywords inside headings, links, etc. than keywords included in non-semantic ```<div>```s, etc., so your documents will be more findable by customers.

Let's get on and look at accessible HTML in more detail.

If you try navigating through a code with good semantic, you'll see that this is pretty easy to navigate:

- The screen reader reads each header out as you progress through the content, notifying you what a heading is, what is a paragraph, etc.
- It stops after each element, letting you go at whatever pace is comfortable for you.
- You can jump to the next/previous heading in many screen readers.
- You can also bring up a list of all headings in many screen readers, allowing you to use them as a handy table of contents to find specific content.

## Best Practices
**Use Container Elements for Layout Only**
Elements like ```<div>``` and ```<span>``` are for layout only. They’re semantically meaningless, they don’t have a keyboard or touch support in any browser, and they don’t communicate anything to the accessibility API. For example, never use a div or span for a button when you could use a semantically meaningful button element.

**Use Other HTML Elements the Way They’re Intended**
All of the other HTML elements should be used to tell the browser what functional purpose your content serves. These other HTML elements provide meaning to the browser and assistive technology about what you’re saying on your website, so you should choose them based on what the content is - not based on how they look with graphics.

**HTML elements to structure every page:**
- header
- nav
- main
- article
- aside
- footer

**Headings**
- Use one H1 per page, matching the page title.
- Do not skip heading levels when increasing, but you can skip levels when decreasing (h1, h2, h3, h2, h3, h4, h2, h3, h4).
- The headings taken out of context should logically represent the page content for screen readers and users who choose this option as a way to scan the page.

**Images and multimedia**

When a screen reader encounters the image, it reads out the full alt attribute — "A red Tyrannosaurus Rex: A two-legged dinosaur standing upright like a human, with small arms, and a large head with lots of sharp teeth.".
This highlights the importance of not only using meaningful file names in case so-called ```alt``` text is not available but also making sure that ```alt``` text is provided in alt attributes wherever possible. Note that the contents of the alt attribute should always provide a direct representation of the image and what it conveys visually. Any personal knowledge or extra description shouldn't be included here, as it is not useful for people who have not come across the image before.

### Links

- https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML
- https://developer.mozilla.org/en-US/
- https://developer.mozilla.org/es/docs/Web/Accessibility/ARIA
- http://web-accessibility.carnegiemuseums.org/foundations/semantic/
- http://simplyaccessible.com/article/pitfalls-info-relationships/
- https://www.interaction-design.org/literature/topics/accessibility
- https://www.w3schools.com/html/html5_semantic_elements.asp
- https://developer.mozilla.org/en-US/docs/Glossary/Semantics
- https://www.freecodecamp.org/news/semantic-html5-elements/