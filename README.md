### Basic-HTML-learning
### <span style="color: Teal;"><strong>HTML learning</strong></span><br>
// Just trying to learn some basic coding, started with Free Code Camp ^^
<a href="https://mcjoules.github.io/html-learning" style="color: DarkSeaGreen;">Main Page</a>;
<a href="https://mcjoules.github.io/html-learning/htmlbasic" target="_blank" style="color: Teal;"> HTML Build Project</a>

// I am trying to put what I have learnt into this little web build project, starting from basic HTML tags, elements and CSS attributes. I also put comments within my code to help me learn. Being able to see the <b>output</b> of my code and experience <b>progress</b> motivates me to continue to learn coding.

Credit to <a href="https://www.freecodecamp.org/" target="_blank" style="color: MidnightBlue">FreeCodeCamp<a>

---
### **Progress**

#### - Basic HTML ####
*h1-h6, comment, href, #, target, body, div, html, img, alt, ul, ol, li, form, action, label, value, name, radio, checkbox, input, text, button, submit, placeholder, required, br*
<br></br>
**Coolest thing I learnt:** `form` element with submit button

  ```html
    <form action="/url-where-to-submit-form-data">
      <input type="text" value="textbox" placeholder="Text here" required> <!--required attribute, required before submit-->
      <button type="submit">Submit</button> <!--submit button!!!-->
    </form>
  ```

**Things I struggled with:** writing in correct HTML structure, understanding the line spacing in certain elements and keeping child of element organised using correct indentation

  ```html
    <!doctype HTML>
    <html>
      <head>
        <title>title</title>
        <style>/*CSS*/</style>
      </head>
      <body>
        <h1>header</h1>
        <main>
          <p>content</p>
        </main>
      </body>
      <footer>footer</footer>
    </html>
  ```
<br/>  

#### - Basic CSS ####
*style, color, margin, class*
<br></br>
**Coolest thing I learnt:** CSS `class` attribute, Google-font import

  ```css
    /*CSS style class attribute*/
    .class-value {
      color: rgb(80,80,80);
      margin: 0;
      font-size: 15px;
      font-family: "Consolas", monaco, monospace;
    }
  ```

**Treasure discovery:** `meta` responsive web development - setting viewport <br>
Credit to <a href="https://www.w3schools.com/css/css_rwd_viewport.asp" target="_blank">w3schools</a>

  ```html
    <!--meta wonder for mobile devices experience-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  ```

**Things I struggled with:** keeping the class attribute tidy, knowing which tags to apply class attribute and Markdown elements for README.md
