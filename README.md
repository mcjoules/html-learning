# Basic-HTML-learning

**GitHub**  
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/mcjoules/html-learning?color=brightgreen&logo=Github)
![GitHub commits since latest release by date (including pre-releases)](https://img.shields.io/github/commits-since/mcjoules/html-learning/v1.0.0?color=brightgreen&include_prereleases&logo=Github)
![GitHub closed issues](https://img.shields.io/github/issues-closed/mcjoules/html-learning?logo=GitHub&color=brightgreen)  

**Languages**  
<a href="https://html.spec.whatwg.org/" target="_blank"><img alt="HTML" src="https://img.shields.io/static/v1?label=HTML&message=build&color=green&logo=HTML5"></a>
<a href="https://www.w3.org/Style/CSS/Overview.en.html" target="_blank"><img alt="CSS" src="https://img.shields.io/static/v1?label=CSS&message=build&color=green&logo=CSS3"></a>
<a href="https://daringfireball.net/projects/markdown/" target="_blank"><img alt="Markdown" src="https://img.shields.io/static/v1?label=Markdown&message=build&color=green&logo=Markdown"></a>  

**Editors**  
<a href="https://atom.io/" target="_blank"><img alt="Atom" src="https://img.shields.io/static/v1?label=Atom&message=editor&color=teal&logo=Atom"></a>
<a href="https://code.visualstudio.com/" target="_blank"><img alt="VS Code" src="https://img.shields.io/static/v1?label=VS%20Code&message=editor&color=teal&logo=Visual%20Studio%20Code"></a>
<a href="https://typora.io/" target="_blank"><img alt="Typora" src="https://img.shields.io/static/v1?label=Typora&message=editor&color=teal&logo="></a>

**Resources**  
<a href="https://www.freecodecamp.org/" target="_blank"><img alt="freeCodeCamp" src="https://img.shields.io/static/v1?label=freeCodeCamp&message=resource&color=yellow&logo=freeCodeCamp"></a>
<a href="https://www.codecademy.com/learn" target="_blank"><img alt="Codecademy" src="https://img.shields.io/static/v1?label=Codecademy&message=resource&color=yellow&logo=Codecademy"></a>
<a href="https://stackoverflow.com/" target="_blank"><img alt="stack overflow" src="https://img.shields.io/static/v1?label=StackOverflow&message=resource&color=yellow&logo=StackOverflow"></a>
<a href="https://docs.github.com/en" target="_blank"><img alt="GitHub Doc" src="https://img.shields.io/static/v1?label=GitHub%20Doc&message=resources&color=yellow&logo=GitHub&link=https://docs.github.com/en&link=%27#"></a>  

I am trying to put what I have learnt into this little web build project, starting from basic HTML tags, elements and CSS attributes. I also put comments within my code to help me learn. Being able to see the **output** of my code and experience **progress** motivates me to continue to learn coding. A lot of my effort will be going into building my **learning notes** besides my project. Writing down notes help me tremendously in my learning.  

## Project

[Html-learning Repo](https://github.com/mcjoules/html-learning)  
[Learning Note](https://github.com/mcjoules/html-learning/tree/main/learning-notes)  
[Repo GitHub Page](https://mcjoules.github.io/html-learning)  
[Repo Wiki](https://github.com/mcjoules/html-learning/wiki)  
[HTML Build Project](https://mcjoules.github.io/html-learning/web-build-project/htmlbasic.html)  
[HTML Build Project - c](https://mcjoules.github.io/html-learning/web-build-project/htmlbasic-c)  

**Table of Content**

- [Basic-HTML-learning](#basic-html-learning)
  - [Project](#project)
  - [Progress](#progress)
    - [Basic HTML](#basic-html)
    - [Basic CSS](#basic-css)
    - [Markdown](#markdown)
    - [Editors and settings](#editors-and-settings)
    - [GitHub](#github)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## Progress

### Basic HTML

_h1-h6, comment, href, #, target, body, div, html, img, alt, ul, ol, li, form, action, label, value, name, radio, checkbox, input, text, button, submit, placeholder, required, br, align_
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

---

### Basic CSS

_style, color: color_name, rgb value, margin, class, margin, border-color, border-width, border-style, border-radius, font-size, font-family: FAMILY_NAME, GENERIC_NAME;, img {height:;width:;}, background-color_
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
Credit to [w3schools](https://www.w3schools.com/css/css_rwd_viewport.asp)  

```html
  <!--meta wonder for mobile devices experience-->
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
```

**Things I struggled with:** keeping the class attribute tidy, knowing which tags to apply class attribute, utilise the many available attributes

---

### Markdown

_code box, dropdowns, table of content [TOC], horizontal line, shield.io badge_
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

---

### Editors and settings

*Extenions, settings, fonts, themes, lint, live-servers, previews, json, shortcuts*  

**Coolest Thing I learnt:** Using both Atom and VS Code, applying extensions, local live-server, shortcuts to stage, commit, and push. Using terminal.  

**Things I struggle with:** Dealing with settings in VS Code extensions, Atom packages and configurations, using json files, ruby files, for custom configs. Using lint. Following the documentations and instructions, using terminal commands. It has been a significant struggle for a beginner. Glad to finally manage to setup linter for both VS Code and Atom and was able to configure the rules, after many late evenings. Example to configure and ignore specific lint rule in markdown:  

```json
{
    "MD033": false,
    "MD014": false
}
```

---

### GitHub

*Repository, GitHub Page, GitHub Markdown, Wiki, Issue, Issue template, GitHub Desktop, GitHub Doc, GitHub with Editors (push and pull), branch, fork, merge*

**Coolest Thing I learnt:** Building my own web-build project and documenting what I have learnt. Discovering the power of GitHub.  

**Things I struggle with:** Using GitHub Markdown, understanding releases and packages, actions, projects, workflow and docker. GitHub Doc does help with its amazing documentation.  
