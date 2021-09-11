[TOC]

# Responsive Web Design

## HTML

### Headings

Opening tags look like this:

```html
<h1>
```

Closing tags look like this:

```html
</h1>
```

//Hello World! Output:

```html
<h1>Hello World!</h1>
<h2>I am Tom.</h2>
```

This element tells the browser about the structure of your website. `h1` elements are often used for main headings, while `h2` elements are generally used for subheadings. There are also `h3`, `h4`, `h5` and `h6` elements to indicate different levels of subheadings.

`p` elements are the preferred element for paragraph text on websites. `p` is short for "paragraph".

```html
<h1>Hello World</h1>
<h2>CatPhotoApp</h2>
<p>Hello Paragraph</p>
```



### Comments in HTML start with `<!--` and end with a `-->`

```html
<!-- This is a comment in HTML -->
```

HTML5 introduces more descriptive HTML tags. These include `main`, `header`, `footer`, `nav`, `video`, `article`, `section` and others.

These tags give a descriptive structure to your HTML, make your HTML easier to read, and help with Search Engine Optimization (SEO) and accessibility. The `main` HTML5 tag helps search engines and other developers find the main content of your page.

```html
<main>
<p>Lorem Ipsum</p>
<p>Lorem Ipsum2</p>
</main>
```

You can add images to your website by using the `img` element, and point to a specific image's URL using the `src` attribute. Note that `img` elements are self-closing. All `img` elements **must** have an `alt` attribute. The text inside an `alt` attribute is used for screen readers to improve accessibility and is displayed if the image fails to load.

**Note:** If the image is purely decorative, using an empty `alt` attribute is a best practice. Ideally the `alt` attribute should not contain special characters unless needed.

```html
<img src="https://www.freecatphotoapp.com/your-image.jpg" alt="A business cat wearing a necktie.">
<img src="https://www.bit.ly/fcc-relaxing-cat" alt="A relaxing cat.">
```

You can use `a` (*anchor*) elements to link to content outside of your web page. `a` elements need a destination web address called an `href` attribute. They also need anchor text.

```html
<a href="https://www.freecodecamp.org">this links to freecodecamp.org</a>
<a href="https://www.freecatphotoapp.com"> cat photos </a>
```



### Link to Internal Sections of a Page with Anchor Elements

`a` (*anchor*) elements can also be used to create internal links to jump to different sections within a webpage.

To create an internal link, you assign a link's `href` attribute to a hash symbol `#` plus the value of the `id` attribute for the element that you want to internally link to, usually further down the page. You then need to add the same `id` attribute to the element you are linking to. An `id` is an attribute that uniquely describes an element.

Below is an example of an internal anchor link and its target element:

```html
<a href="#contacts-header">Contacts</a>
<h2 id="contacts-header">Contacts</h2>
```

When users click the `Contacts` link, they'll be taken to the section of the webpage with the **Contacts** header element.
`#` create an internal link, `target="_blank"` cause it to open a new window tab

```html
 <a href="#footer" target="_blank">cat photos</a>
```

//Create a `Jump to Bottom` internal link with the `footer` element. It is **important** to `id` the footer element, or other elements.

```html
<main>
  <a href="#footer">Jump to Bottom</a>
  ...
</main>
<footer id="footer">Copyright Cat Photo App</footer>
```



### The Body

One of the key HTML elements we use to build a webpage is the *body* element. Only content inside the opening and closing body tags can be displayed to the screen. Here’s what opening and closing body tags look like:

```html
<body>
</body>
```

Once the file has a body, many different types of content – including text, images, and buttons – can be added to the body.

```html
<body>
  <p>What's up, doc?</p>
</body>
```



### Differences between main and body:

**main**:

> The content inside the **main** element should be unique to the document. It should not contain any content that is repeated across documents such as sidebars, navigation links, copyright information, site logos, and search forms.

**body**:

> The **body** element contains all the contents of an HTML document, such as text, hyperlinks, images, tables, lists, etc.

An easy example, the footer element; you should put it inside the body, but outside the main, as you will do with your menu, or sidebar.



### `<div>` Div Element

The `<div>` element is used as a container that divides an HTML document into sections and is short for “division”. `<div>` elements can contain *flow content* such as headings, paragraphs, links, images, etc.

```html
<div>
  <h1>A section of grouped elements</h1>
  <p>Here’s some text for the section</p>
</div>
<div>
  <h1>Second section of grouped elements</h1>
  <p>Here’s some text</p>
</div>
```



### `<html>` HTML Element

The `<html>` element, the root of an HTML document, should be added after the `!DOCTYPE` declaration. All content/structure for an HTML document should be contained between the opening and closing `<html>` tags.

```html
<!DOCTYPE html>
<html>
  <!-- I'm a comment -->
</html>
```



### Make Dead Links Using the Hash Symbol

Add `a` elements to your website before you know where they will link. This is also handy when you're changing the behaviour of a link using `JavaScript`. For example: `href="#"`

```html
<!--dead link--> 
<p>View more <a href="#" target="_blank">cat photos</a>.</p>
```



### Turn an Image into a Link `with a dead link`

You can make elements into links by nesting them within an `a` element. Nest your image within an `a` element. Here's an example:

```html
<a href="#"><img src="https://www.bit.ly/fcc-running-cats" alt="Three kittens running towards the camera."></a>
```

Remember to use `#` as your `a` element's `href` property in order to turn it into a dead link.



### Create a Bulleted Unordered List

HTML has a special element for creating unordered lists, or bullet point style lists. Unordered lists start with an opening `<ul>` element, followed by any number of `<li>` elements. Finally, unordered lists close with a `</ul>`. For example:

```html
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```



### Create an Ordered List

HTML has another special element for creating ordered lists, or numbered lists. Ordered lists start with an opening `<ol>` element, followed by any number of `<li>` elements. Finally, ordered lists are closed with the `</ol>` tag. For example:

```html
<ol>
  <li>Garfield</li>
  <li>Sylvester</li>
</ol>
```

would create a numbered list of `Garfield` and `Sylvester`.



### Create a Text Field

`input` elements are a convenient way to get input from your user. You can create a text input like this:

```html
<input type="text">
<p>Input type="text"<input type="text" placeholder="text here"></p>
<p>Input type="date"<input type="date"></p>
```

Note that `input` elements are self-closing.



### Add Placeholder Text to a Text Field

Placeholder text is what is displayed in your `input` element before your user has inputted anything. You can create placeholder text like so:

```html
<input type="text" placeholder="this is placeholder text">
```



### Create a Form Element

`form` element. For example:

```html
<form action="/url-where-you-want-to-submit-form-data">
    <input type="text" placeholder="Text here">
</form>
```



### Add a Submit Button to a Form

Here's an example submit button: put it within the form element

```html
<button type="submit">Submit</button>
```



### Use HTML5 to Require a Field

```html
<form action="/url-where-to-submit-form-data">
      <input type="text" placeholder="Text here" required>
      <button type="submit">Submit</button>
</form>
```

For example, if you wanted to make a text input field required, you can just add the attribute `required` within your `input` element, like this: `<input type="text" required>`



### Create a Set of Radio Buttons

```html
<!--Radio buttons-->
<label for="indoor">
  <input id="indoor" type="radio" name="indoor-outdoor"> Indoor</label>
<label for="outdoor">
  <input id="outdoor" type="radio" name="indoor-outdoor"> Outdoor</label>
```



### Create a Set of Checkboxes

```html
  <!-- checkbox input element-->
      <label for="Coffee">
        <input id="Coffee" type="checkbox" name="morning"> Coffee</label>
      <label for="Breakfast">
        <input id="Breakfast" type="checkbox" name="morning"> Breakfast</label>
      <label for="Dress">
        <input id="Dress" type="checkbox" name="morning"> Dress</label>
```



### Use the value attribute with Radio Buttons and Checkboxes

When a form gets submitted, the data is sent to the server and includes entries for the options selected. Inputs of type `radio` and `checkbox` report their values from the `value` attribute. For example:

```html
<label for="indoor">
  <input id="indoor" value="indoor" type="radio" name="indoor-outdoor">Indoor</label>
<label for="outdoor">
  <input id="outdoor" value="outdoor" type="radio" name="indoor-outdoor">Outdoor</label>
```



### Check Radio Buttons and Checkboxes by Default

You can set a checkbox or radio button to be checked by default using the `checked` attribute. To do this, just add the word `checked` to the inside of an input element. For example:

```html
<input type="radio" name="test-name" checked>
```



### Nest Many Elements within a Single div Element

The `div` element, also known as a division element, is a general purpose container for other elements.
The `div` element is probably the most commonly used HTML element of all.



### Declare the Doctype of an HTML Document

At the top of your document, you need to tell the browser which version of HTML your page is using. HTML is an evolving language, and is updated regularly. Most major browsers support the latest specification, which is HTML5. However, older web pages may use previous versions of the language.

You tell the browser this information by adding the `<!DOCTYPE ...>` tag on the first line, where the `...` part is the version of HTML. For HTML5, you use `<!DOCTYPE html>`.

The `!` and uppercase `DOCTYPE` is important, especially for older browsers. The `html` is not case sensitive.

Next, the rest of your HTML code needs to be wrapped in `html` tags. The opening `<html>` goes directly below the `<!DOCTYPE html>` line, and the closing `</html>` goes at the end of the page.

Here's an example of the page structure. Your HTML code would go in the space between the two `html` tags.

```html
<!DOCTYPE html>
<html>
</html>
```



### Define the Head and Body of an HTML Document

You can add another level of organization in your HTML document within the `html` tags with the `head` and `body` elements. Any markup with information about your page would go into the `head` tag. Then any markup with the content of the page (what displays for a user) would go into the `body` tag.

Metadata elements, such as `link`, `meta`, `title`, and `style`, typically go inside the `head` element.

Here's an example of a page's layout:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta />
  </head>
  <body>
    <div>
    </div>
  </body>
</html>
```



### Align text

[Alignment, font styles, and horizontal rules in HTML documents (w3.org)](https://www.w3.org/TR/html401/present/graphics.html)

```html
<p align="justify">paragraph</p>
```



### Adding a shield.io badge 

![name](https://img.shields.io/static/v1?label=shields.io&message=badge&color=<color>&logo=Shields.io)
[GitHub: How to add Shields | Easy, visible info on your projects - YouTube](https://www.youtube.com/watch?v=Dl-ekLb4quE&ab_channel=TroubleChute)
[Shields.io: Quality metadata badges for open source projects](https://shields.io/#your-badge)

Study the web link address carefully, input in place of <input> and remove the <> as well. Select the categories in the shields.io website for interactive, dynamic badges linked to GitHub

**Markdown:**

```markdown
<!--https://shields.io/--> <!--Markdown-->
![name](https://img.shields.io/static/v1?label=<label>&message=<message>&color=<color>&logo=<name>)
```

**HTML:**

```html
<!--https://shields.io/--> <!--HTML-->
<img alt="alt-text" src="https://img.shields.io/static/v1?label=<label>&message=<message>&color=<color>&logo=<name>">

<!--to make the badge into a link using anchor href-->
<a href="https://atom.io/" target="_blank"><img alt="Atom shields.io" src="https://img.shields.io/static/v1?label=Atom&message=editor&color=teal&logo=Atom"></a>
```

**Activity: version**
Click on the categories, e.g. activity, version is the release version tag e.g. `v1.0.0`, shield.io will automatically check if the version exist or not.
