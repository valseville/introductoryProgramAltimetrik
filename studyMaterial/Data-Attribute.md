# Data-Attribute
Are additional values that configure the elements or adjust their behavior in various ways to meet the criteria the users want.

HTML5 is designed with extensibility in mind for data that should be associated with a particular element but need not have any defined meaning. ```data-*``` attributes allow us to store extra information on standard, semantic HTML elements without other hacks such as non-standard attributes, or extra properties on DOM.

The syntax is simple. Any attribute on any element whose attribute name starts with ```data-``` is a data attribute. Say you have an article and you want to store some extra information that doesn't have any visual representation. Just use data attributes for that:

```<article```  

 ``` id="electric-cars"```  

 ``` data-columns="3"```  

 ``` data-index-number="12314"```  

  ```data-parent="cars">```  

```...```  

```</article>```

You can also use the values of the data-attributes with JavaScript in fact it’s pretty easy to read these values. You could use ```getAttribute()``` with their full HTML name to read them, but the standard defines a simpler way: a ```DOMStringMap``` you can read out via a dataset property.

To get a ```data``` attribute through the ```dataset ``` object, get the property by the part of the attribute name after ```data-``` (note that dashes are converted to camelCase).

```const article = document.querySelector('#electric-cars');```  

```// The following would also work:```  

```// const article = document.getElementById("electric-cars")```  

```article.dataset.columns // "3"```  

```article.dataset.indexNumber // "12314"```  

```article.dataset.parent // "cars"```

## Links
- https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes