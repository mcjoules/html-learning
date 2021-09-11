<h3><a name="title" style="color: Teal;"><b>Basic-HTML-learning</b></a></h3>

<img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/m/mcjoules/html-learning?color=brightgreen&logo=github"> <img alt="GitHub commits since latest release (by date including pre-releases)" src="https://img.shields.io/github/commits-since/mcjoules/html-learning/v1.0.0?color=brightgreen&include_prereleases&logo=github">
<a href="https://html.spec.whatwg.org/" target="_blank"><img alt="HTML shield.io" src="https://img.shields.io/static/v1?label=HTML&message=build&color=green&logo=HTML5"></a>
<a href="https://www.w3.org/Style/CSS/Overview.en.html" target="_blank"><img alt="CSS shield.io" src="https://img.shields.io/static/v1?label=CSS&message=build&color=green&logo=CSS3"></a>
<a href="https://daringfireball.net/projects/markdown/" target="_blank"><img alt="Markdown shield.io" src="https://img.shields.io/static/v1?label=Markdown&message=build&color=green&logo=Markdown"></a>
<a href="https://atom.io/" target="_blank"><img alt="Atom shield.io" src="https://img.shields.io/static/v1?label=Atom&message=editor&color=teal&logo=Atom"></a>
<a href="https://code.visualstudio.com/" target="_blank"><img alt="VS Code shield.io" src="https://img.shields.io/static/v1?label=VS%20Code&message=editor&color=teal&logo=Visual%20Studio%20Code"></a>
<a href="https://typora.io/" target="_blank"><img alt="Typora shield.io" src="https://img.shields.io/static/v1?label=Typora&message=editor&color=teal&logo="></a>
<a href="https://www.freecodecamp.org/" target="_blank"><img alt="freeCodeCamp shield.io" src="https://img.shields.io/static/v1?label=freeCodeCamp&message=course&color=yellow&logo=freeCodeCamp"></a>
<a href="https://www.codecademy.com/learn" target="_blank"><img alt="Codecademy shield.io" src="https://img.shields.io/static/v1?label=Codecademy&message=course&color=yellow&logo=Codecademy"></a>

### <a name="introduction"><span><strong>HTML learning Introduction</strong></span></a><br>
// Just trying to learn some basic coding, started with Free Code Camp ^^<br>
<a href="https://mcjoules.github.io/html-learning" style="color: DarkSeaGreen;">Main Page</a>;<br>
<a href="https://mcjoules.github.io/html-learning/web-build-project/htmlbasic.html" target="_blank" style="color: Teal;"> HTML Build Project</a>

// I am trying to put what I have learnt into this little web build project, starting from basic HTML tags, elements and CSS attributes. I also put comments within my code to help me learn. Being able to see the <b>output</b> of my code and experience <b>progress</b> motivates me to continue to learn coding.

Credit to <a href="https://www.freecodecamp.org/" target="_blank" style="color: MidnightBlue">FreeCodeCamp<a>

<br/>

<h3>Table of Contents</h3>

* [Introduction](#introduction)
* [Progress](#progress)
    * [Basic HTML](#basic-html)
    * [Basic CSS](#basic-css)
    * [Markdown](#markdown)
<br/>
<br/>


---
### <a name="progress"><b>Progress</b></a>

#### <a name="basic-html">Basic HTML</a> ####
*h1-h6, comment, href, #, target, body, div, html, img, alt, ul, ol, li, form, action, label, value, name, radio, checkbox, input, text, button, submit, placeholder, required, br, align*
<br/>

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
<br/>

#### <a name="basic-css">Basic CSS</a> ####
*style, color: color_name, rgb value, margin, class, margin, border-color, border-width, border-style, border-radius, font-size, font-family: FAMILY_NAME, GENERIC_NAME;, img {height:;width:;}, background-color*
<br/>

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

**Things I struggled with:** keeping the class attribute tidy, knowing which tags to apply class attribute, utilise the many available attributes
<br/>
<br/>
<br/>

#### <a name="markdown">Markdown</a> ####
*code box, dropdowns, table of content [TOC], horizontal line, shield.io badge*
<br/>

**Coolest thing I learn:** Table of Contents

  ```markdown
  Table of Contents
  =================
  * [Topic](#class-name)
  <a href="class-name">Topic</a>
  ```

**Treasure discovery:** shied.io badge ![shields.io](https://img.shields.io/static/v1?label=shields.io&message=badge&color=%3Cbrightgreen%3E&logo=Shields.io)

   ```markdown
  <!--https://shields.io/-->
  ![name](https://img.shields.io/static/v1?label=<label>&message=<message>&color=<color>&logo=<name>)
  ```

**Things I struggle with:** understanding markdown syntax, markdown spacing and line break, working between md syntax and html [what work and what doesn't work], discovering the affects and relation of md syntax and html, keeping codes tidy and well structured.
