➥ ./gh-md-toc https://github.com/ekalinin/envirius/blob/master/README.md

Table of Contents
=================

  * [envirius](#envirius)
    * [Idea](#idea)
    * [Features](#features)
  * [Installation](#installation)
  * [Uninstallation](#uninstallation)
  * [Available plugins](#available-plugins)
  * [Usage](#usage)
    * [Check available plugins](#check-available-plugins)
    * [Check available versions for each plugin](#check-available-versions-for-each-plugin)
    * [Create an environment](#create-an-environment)
    * [Activate/deactivate environment](#activatedeactivate-environment)
      * [Activating in a new shell](#activating-in-a-new-shell)
      * [Activating in the same shell](#activating-in-the-same-shell)
    * [Get list of environments](#get-list-of-environments)
    * [Get current activated environment](#get-current-activated-environment)
    * [Do something in environment without enabling it](#do-something-in-environment-without-enabling-it)
    * [Get help](#get-help)
    * [Get help for a command](#get-help-for-a-command)
  * [How to add a plugin?](#how-to-add-a-plugin)
    * [Mandatory elements](#mandatory-elements)
      * [plug_list_versions](#plug_list_versions)
      * [plug_url_for_download](#plug_url_for_download)
      * [plug_build](#plug_build)
    * [Optional elements](#optional-elements)
      * [Variables](#variables)
      * [Functions](#functions)
    * [Examples](#examples)
  * [Example of the usage](#example-of-the-usage)
  * [Dependencies](#dependencies)
  * [Supported OS](#supported-os)
  * [Tests](#tests)
  * [Version History](#version-history)
  * [License](#license)
  * [README in another language](#readme-in-another-language)


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

#### - Basic CSS ####
*style, color, margin, class*
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

**Things I struggled with:** keeping the class attribute tidy, knowing which tags to apply class attribute, utilise the many available attributes, Markdown elements for README.md
