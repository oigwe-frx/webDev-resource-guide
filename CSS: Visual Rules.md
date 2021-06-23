## Font Family

Font refers to the technical term typeface, or font family.

To change the typeface of text on your web page, you can use the font-family property.

```
h1 {
  font-family: Garamond;
}
```

In the example above, the font family for all main heading elements has been set to Garamond.

When setting typefaces on a web page, keep the following points in mind:

The font specified must be installed on the user’s computer or downloaded with the site.
Web safe fonts are a group of fonts supported across most browsers and operating systems.
Unless you are using web safe fonts, the font you choose may not appear the same between all browsers and operating systems.
When the name of a typeface consists of more than one word, it’s a best practice to enclose the typeface’s name in quotes, like so:

```
h1 {
  font-family: 'Courier New';
}
```


## Text Align

No matter how much styling is applied to text (typeface, size, weight, etc.), the text always appears on the left side of the container in which it resides.

To align text we can use the text-align property. The text-align property will align text to the element that holds it, otherwise known as its parent.

```
h1 {
  text-align: right;
}
```

The text-align property can be set to one of the following commonly used values:

- left — aligns text to the left side of its parent element, which in this case is the browser.
- center — centers text inside of its parent element.
- right — aligns text to the right side of its parent element.
- justify— spaces out text in order to align with the right and left side of the parent element.

## Opacity
Opacity is the measure of how transparent an element is. It’s measured from 0 to 1, with 1 representing 100%, or fully visible and opaque, and 0 representing 0%, or fully invisible.

Opacity can be used to make elements fade into others for a nice overlay effect. To adjust the opacity of an element, the syntax looks like this:

```
.overlay {
  opacity: 0.5;
}
```


## Background Image

CSS has the ability to change the background of an element. One option is to make the background of an element an image. This is done through the CSS property background-image. Its syntax looks like this:

```
.main-banner {
  background-image: url('https://www.example.com/image.jpg');
}
```
The background-image property will set the element’s background to display an image.
The value provided to background-image is a url. The url should be a URL to an image. The url can be a file within your project, or it can be a link to an external site. To link to an image inside an existing project, you must provide a relative file path. If there was an image folder in the project, with an image named mountains.jpg, the relative file path would look like below:

```
.main-banner {
  background-image: url('images/mountains.jpg')
}
```

## Important

!important can be applied to specific declarations, instead of full rules. It will override any style no matter how specific it is. As a result, it should almost never be used. Once !important is used, it is very hard to override.

The syntax of !important in CSS looks like this:

```

p {
  color: blue !important;
}
 
.main p {
  color: red;
}

```

Since !important is used on the p selector’s color attribute, all p elements will appear blue, even though there is a more specific .main p selector that sets the color attribute to red.

One justification for using !important is when working with multiple stylesheets. For example, if we are using the Bootstrap CSS framework and want to override the styles for one specific HTML element, we can use the !important property.
