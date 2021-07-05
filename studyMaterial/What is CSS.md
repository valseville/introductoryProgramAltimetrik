# What is CSS?
The CSS acronym stands for cascade style sheets, it defines how HTML elements are going to look like. Allows us to make a clear separation between content and style. HTML is the content and CSS is the style of the content. You can use CSS in 3 different ways:

- CSS code inside and HTML Tag using the style attribute
- We can write CSS code in the head section of the HTML document 
- CSS code can be put in an external file

The better way it’s the last one, you can have a clear separation between style and content, and your documents are going to be cleaner.

CSS is written in rules, each rule consists of a selector and a declaration block, we can attribute class or ID names to elements and then use these classes or IDs to select them. You can have many classes with the same name as you want but the IDs are unique; you can only use one name per ID.

**Specificity**
Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied. Specificity is based on the matching rules which are composed of different sorts of CSS selectors.

**How is specificity calculated?**
Specificity is a weight that is applied to a given CSS declaration, determined by the number of each selector type in the matching selector. When multiple declarations have equal specificity, the last declaration found in the CSS is applied to the element. Specificity only applies when the same element is targeted by multiple declarations. As per CSS rules, directly targeted elements will always take precedence over rules which an element inherits from its ancestor.

**Selector Types**
The following list of selector types increases by specificity:

- Type selectors (e.g., h1) and pseudo-elements (e.g., ::before).
- Class selectors (e.g., .example), attributes selectors (e.g., [type="radio"]) and pseudo-classes (e.g., :hover).
- ID selectors (e.g., #example).
- Universal selector (*), combinators (+, >, ~, ' ', ||) and negation pseudo-class (:not()) have no effect on specificity. (The selectors declared inside :not() do, however.)


Inline styles added to an element (e.g., style="font-weight: bold;") always overwrite any styles in external stylesheets, and thus can be thought of as having the highest specificity.

**The !important exception**
When an important rule is used on a style declaration, this declaration overrides any other declarations. Although technically !important has nothing to do with specificity, it interacts directly with it. Using !important, however, is bad practice and should be avoided because it makes debugging more difficult by breaking the natural cascading in your stylesheets. When two conflicting declarations with the !important rule are applied to the same element, the declaration with a greater specificity will be applied.

**Some rules of thumb:**
- Always look for a way to use specificity before even considering !important
- Only use !important on page-specific CSS that overrides foreign CSS (from external libraries, like Bootstrap or normalize.css).
- Never use !important when you're writing a plugin/mashup.
- Never use !important on site-wide CSS.

**Box Model**
All the HTML elements can be seen as boxes, the box model allows us to define space between elements and to add a border around elements. The box model consists of margins, padding, borders and actual content of the box.

![](https://media.gcflearnfree.org/content/5ef2084faaf0ac46dc9c10be_06_23_2020/box_model.png)

The **content area**, bounded by the content edge, contains the "real" content of the element, such as text, an image, or a video player. Its dimensions are the content width (```or content-box width```) and the content height (or ```content-box height```). It often has a background color or background image.

If the ```box-sizing property``` is set to ```content-box``` (default) and if the element is a block element, the content area's size can be explicitly defined with the ```width```, ```min-width```, ```max-width```, ```height```, ```min-height```, and ```max-height``` properties.

The **padding** area, bounded by the padding edge, extends the content area to include the element's padding. Its dimensions are the padding-box width and the padding-box height.
The thickness of the padding is determined by the ```padding-top```, ```padding-right```, ```padding-bottom```, ```padding-left```, and shorthand ```padding``` properties.

The **border** area, bounded by the border edge, extends the padding area to include the element's borders. Its dimensions are the border-box width and the border-box height.

The thickness of the borders are determined by the ```border-width``` and shorthand border properties. If the ```box-sizing``` property is set to ```border-box```, the border area's size can be explicitly defined with the ```width```, ```min-width```, ```max-width```, ```height```, ```min-height```, and ```max-height``` properties. When there is a background (```background-color``` or ```background-image```) set on a box, it extends to the outer edge of the border (i.e. extends underneath the border in z-ordering). This default behavior can be altered with the ```background-clip``` css property.

The margin area, bounded by the margin edge, extends the border area to include an empty area used to separate the element from its neighbors. Its dimensions are the margin-box width and the margin-box height.

The size of the margin area is determined by the ```margin-top```, ```margin-right```, ```margin-bottom```, ```margin-left```, and shorthand margin properties. When margin collapsing occurs, the margin area is not clearly defined since margins are shared between boxes.

Finally, note that for non-replaced inline elements, the amount of space taken up (the contribution to the height of the line) is determined by the ```line-height``` property, even though the borders and padding are still displayed around the content.

The ```box-sizing``` CSS property sets how the total width and height of an element is calculated.

## Links

- https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity
- https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance
- https://developer.mozilla.org/en-US/docs/Learn/CSS

 