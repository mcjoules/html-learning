- [CSS Basic](#css-basic)
    - [Meta for setting Viewport for mobile device](#meta-for-setting-viewport-for-mobile-device)
    - [Change the Color of Text](#change-the-color-of-text)
    - [Use CSS Selectors to Style Elements](#use-css-selectors-to-style-elements)
    - [Use a CSS Class to Style an Element](#use-a-css-class-to-style-an-element)
    - [Style Multiple Elements with a CSS Class](#style-multiple-elements-with-a-css-class)
    - [Change the Font Size of an Element](#change-the-font-size-of-an-element)
    - [Set the Font Family of an Element](#set-the-font-family-of-an-element)
    - [Import a Google Font](#import-a-google-font)
    - [Specify How Fonts Should Degrade](#specify-how-fonts-should-degrade)
    - [Size Your Images](#size-your-images)
    - [Add Borders Around Your Elements](#add-borders-around-your-elements)
    - [Multiple classes](#multiple-classes)
    - [Add Rounded Corners with border-radius](#add-rounded-corners-with-border-radius)
    - [Give a Background Color to a div Element](#give-a-background-color-to-a-div-element)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

# CSS Basic

### Meta for setting Viewport for mobile device

[Responsive Web Design Viewport
(w3schools.com)](https://www.w3schools.com/css/css_rwd_viewport.asp)

HTML5 introduced a method to let web designers take control over the
viewport, through the `<meta>` tag. You should include the following
`<meta>` viewport element in all your web pages:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### Change the Color of Text

[HTML Color Names
(w3schools.com)](https://www.w3schools.com/colors/colors_names.asp)

The property that is responsible for the color of an element's text is
the `color` style property. Here's how you would set your `h2` element's
text color to blue:

```html
<h2 style="color: blue;">CatPhotoApp</h2>
```

Note that it is a good practice to end inline `style` declarations with
a `;` .

### Use CSS Selectors to Style Elements

Inside that style block, you can create a CSS selector for all `h2`
elements. For example, if you wanted all `h2` elements to be red, you
would add a style rule that looks like this:

```html
<style>
  h2 {
    color: red;
  }
</style>
```

Note that it's important to have both opening and closing curly braces
(`{` and `}`) around each element's style rule(s). You also need to make
sure that your element's style definition is between the opening and
closing style tags. Finally, be sure to add a semicolon to the end of
each of your element's style rules.

### Use a CSS Class to Style an Element

Classes are reusable styles that can be added to HTML elements. Here's
an example CSS class declaration:

```html
<style>
  .blue-text {
    color: blue;
  }
</style>
```

You can see that we've created a CSS class called `blue-text` within the
`<style>` tag. You can apply a class to an HTML element like this:
`<h2 class="blue-text">CatPhotoApp</h2>`. Note that in your CSS `style`
element, class names start with a period. In your HTML elements' class
attribute, the class name does not include the period.

### Style Multiple Elements with a CSS Class

Classes allow you to use the same CSS styles on multiple HTML elements.
You can see this by applying your `red-text` class to the first `p`
element.

### Change the Font Size of an Element

Font size is controlled by the `font-size` CSS property, like this:

```css
h1 {
  font-size: 30px;
}
```

### Set the Font Family of an Element

You can set which font an element should use, by using the `font-family`
property.

For example, if you wanted to set your `h2` element's font to
`sans-serif`, you would use the following CSS:

```css
h2 {
  font-family: sans-serif;
}
```

### Import a Google Font

In addition to specifying common fonts that are found on most operating
systems, we can also specify non-standard, custom web fonts for use on
our website. There are many sources for web fonts on the Internet. For
this example we will focus on the Google Fonts library.

[Google Fonts](https://fonts.google.com/) is a free library of web fonts
that you can use in your CSS by referencing the font's URL.

To import a Google Font, you can copy the font's URL from the Google
Fonts library and then paste it in your HTML. We'll import the
`Major Mono Display` font. To do this, copy the following code snippet
and paste it into the top of your code editor (before the opening
`style` element):

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
or
<head>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Major+Mono+Display&display=swap" rel="stylesheet">
</head>
```

You can use the `Major Mono Display` font in your CSS by using
`Major Mono Display` as the FAMILY_NAME as in the following example:

```html
font-family: FAMILY_NAME, GENERIC_NAME;
font-family: 'Major Mono Display', monospace;
```

The GENERIC_NAME is optional - `monospace`, and is a fallback font in
case the other specified font is not available.

Family names are case-sensitive and need to be wrapped in quotes if
there is a space in the name. For example, you need quotes to use the
`"Open Sans"` font, but not to use the `Lobster` font.

### Specify How Fonts Should Degrade

There are several default fonts that are available in all browsers.
These generic font families include `monospace`, `serif` and
`sans-serif`.

When one font isn't available, you can tell the browser to "degrade" to
another font.

For example, if you wanted an element to use the `Helvetica` font, but
degrade to the `sans-serif` font when `Helvetica` isn't available, you
will specify it as follows:

```html
p {
  font-family: Helvetica, sans-serif;
}
```

Generic font family names are not case-sensitive. Also, they do not need
quotes because they are CSS keywords.

### Size Your Images

CSS has a property called `width` that controls an element's width. Just
like with fonts, we'll use `px` (pixels) to specify the image's width.

For example, if we wanted to create a CSS class called `larger-image`
that gave HTML elements a width of 500 pixels, we'd use:

```html
<style>
  .larger-image {
    width: 500px;
  }
</style>
```

### Add Borders Around Your Elements

CSS borders have properties like `style`, `color` and `width`. For
example, if we wanted to create a red, 5 pixel border around an HTML
element, we could use this class:

```html
<style>
  .thin-red-border {
    border-color: red;
    border-width: 5px;
    border-style: solid; /*other styles are available*/
    border-radius: 15px;
  }
</style>
```

### Multiple classes

Remember that you can apply multiple classes to an element using its
`class` attribute, by separating each class name with a space. For
example:

```html
<img class="class1 class2">
```

### Add Rounded Corners with border-radius

You can specify a `border-radius` with pixels. `border-radius` of
`10px`.

```html
<style>
  .thin-red-border {
    border-color: red;
    border-width: 5px;
    border-style: solid;
    border-radius: 15px; /*add round corners*/
  }
</style>
```

### Give a Background Color to a div Element

You can set an element's background color with the `background-color`
property. For example, if you wanted an element's background color to be
`green`, you'd put this within your `style` element:

```html
.green-background {
  background-color: green;
}
```
