# Markdown

- [Markdown](#markdown)
  - [Dropdowns](#dropdowns)
  - [Table of content TOC](#table-of-content-toc)
  - [Empty line break](#empty-line-break)
  - [Italic/ bold/ header](#italic-bold-header)
  - [Making a code fence](#making-a-code-fence)
  - [Adding a shield.io badge](#adding-a-shieldio-badge)
  - [Transfer Typora TOC onto GitHub README.md](#transfer-typora-toc-onto-github-readmemd)
  - [GitHub markdown](#github-markdown)
    - [GitHub page customisation](#github-page-customisation)
    - [GitHub markdown relative links](#github-markdown-relative-links)
  - [Reduce HTML elements in Markdown](#reduce-html-elements-in-markdown)
  - [Beautify and Markdown syntax](#beautify-and-markdown-syntax)
  - [Space after HTML element for markdown syntax](#space-after-html-element-for-markdown-syntax)
  - [Escaping Characters](#escaping-characters)
    - [Backstick in inline code](#backstick-in-inline-code)
  - [Tables in Markdown](#tables-in-markdown)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

[Markdown Cheat Sheet \| Markdown
Guide](https://www.markdownguide.org/cheat-sheet/)

## Dropdowns

```markdown
<details>
  <summary>Topic</summary>
  This text will be hidden.
</details>
```

## Table of content TOC

```markdown
Table of Contents
=================
  * [Topic](#class-name)
  <a href="class-name">Topic</a>
```

## Empty line break

```html
<!--sometimes an empty line break is required, so <br/> does not affect other syntax/elements in markdown-->
<br/>
<br/>
```

## Italic/ bold/ header

```markdown
<!--italic-->*Hello*
<!--bold-->**Hello**
<!--h3-->### Hello ###
```

## Making a code fence

````markdown
    ```html/css/markdown
      <!--insert code here-->
    ```
````

## Adding a shield.io badge

![shields.io](https://img.shields.io/static/v1?label=shields.io&message=badge&color=<color>&logo=Shields.io "fig:")  
[GitHub: How to add Shields \| Easy, visible info on your projects -YouTube](https://www.youtube.com/watch?v=Dl-ekLb4quE&ab_channel=TroubleChute)  
[Shields.io: Quality metadata badges for open source projects](https://shields.io/#your-badge)  

Study the web link address carefully, input in place of `<input>` and remove the `<` and `>` as well. Select the categories in the shields.io website for interactive, dynamic badges linked to GitHub  

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

## Transfer Typora TOC onto GitHub README.md

GitHub markdown uses **pandoc** markdown which differs from Typora markdown. To turn the **Typora** markdown table of content TOC into functional TOC in GitHub, we need to export the Typora file as **Markdown (other spec)**.  

1 - Go to **File > Preferences > Export**  
2 - Add export type as **Markdown (other spec) > variant:
GitHub-flavored markdown**  
3 - Install **pandoc** as instructed  
4 - Restart **PC? or Typora**  
5 - Export your **Typora** file: **File > Export > Markdown (other
spec)**  
6 - Your new file should have TOC that works in GitHub README.md/ GitHub
markdown

## GitHub markdown

**Create TOC in markdown File** - [GitHub TOC Generator](https://ecotrust-canada.github.io/markdown-toc/) by ecotrust-canada  
// Special characters such as \`\` or ** or : will invalidate the TOC link, as TOC generator turn it into `-` character. For example:  

```markdown
[**Atom**](#--atom--) <!--invalid TOC link due to `**` special characters, conversion into `--` characters-->
```

### GitHub page customisation

Example of basic customisation on GitHub page, see [pages-themes minimal](https://github.com/pages-themes/minimal) by parkr:

```yml
remote_theme: pages-themes/minimal@v0.2.0
plugins:
- jekyll-remote-theme # add this line to the plugins list if you already have one
title: html-learning
logo: assets/img/logo_bear2.png
description: Basic HTML, CSS learning with a test web building project to implement what I learnt.
show_downloads: true
google_analytics:
```

### GitHub markdown relative links

Example of creating internal links (relative links) to other markdown (md) notes in repository with markdown, see [stackoverflow GitHub Blog Relative Links](https://stackoverflow.com/questions/7653483/github-relative-link-in-markdown-file/7658676#7658676):

```markdown
[HTML Basics Notes](learning-notes/HTML-Basics-notes.md)  
[CSS Basics Notes](learning-notes/CSS-Basic-notes.md)  
[Markdown Notes](learning-notes/Markdown-notes.md)  
[Editor Notes](learning-notes/Editor-notes.md)  
```

## Reduce HTML elements in Markdown

When possible, avoid using HTML elements in Markdown, e.g. links, italics, bold. Focus on using Markdown syntax.  

## Beautify and Markdown syntax

Beware that **Beautify** may affect some Markdown syntax. Use with caution in Markdown.  

## Space after HTML element for markdown syntax

It is important to have a blank line after HTML element to allow Markdown syntax to function.  

**Incorrect example:**

```html
<details>
  <summary>Wrong</summary>
This is a `wrong example` <!--no blank lines, md syntax will not work-->
</details>
```

**Correct example:**

```html
<details>
  <summary>Correct</summary>

This is a `correct example` <!--add blank lines, md syntax works-->

</details>
```

## Escaping Characters

To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash `\` in front of the character.

See [markdownguide.org - Escaping Characters](https://www.markdownguide.org/basic-syntax/#escaping-characters)

|Character|Name|
|-------|--------|
|`\`|backslash|  
|`` ` ``|backtick|
|`*`|asterisk|
|`_`|underscore|
|`{`,`}`|curly braces|
|`[`,`]`|brackets|
|`<`,`>`|angle brackets|
|`(`,`)`|parentheses|
|`#`|hash|
|`+`|plus sign|
|`-`|hyphen|
|`.`|dot|
|`!`|exclamation mark|
|`\|`|pipe|

### Backstick in inline code

To place the backstick `` ` `` in a inline code, spacing *before* and *after* the `` ` `` is needed, and **double backstick** quote is needed. See example:  

```markdown
`` ` `` //correct
```     //incorrect
`````   //incorrect
```

## Tables in Markdown

See [markdownguide - tables](https://www.markdownguide.org/extended-syntax/#tables)  
To add a table, use three or more hyphens `---` to create each column’s header, and use pipes `|` to separate each column. For compatibility, you should also add a pipe on either end of the row.

```markdown
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

Cell widths can vary, as shown below. The rendered output will look the same.

```markdown
| Syntax | Description |
| --- | ----------- |
| Header | Title |
| Paragraph | Text |
```

**Alignment**
You can align text in the columns to the left, right, or centre by adding a colon `:` to the left, right, or on both side of the hyphens within the header row.

```markdown
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```
