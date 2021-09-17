- [Markdown](#markdown)
    - [Dropdowns](#dropdowns)
    - [Table of content TOC](#table-of-content-toc)
    - [Empty line break](#empty-line-break)
    - [Italic/ bold/ header](#italic-bold-header)
    - [Making a code fence](#making-a-code-fence)
    - [Adding a shield.io badge](#adding-a-shieldio-badge)
    - [Transfer Typora TOC onto GitHub README.md](#transfer-typora-toc-onto-github-readmemd)
    - [GitHub markdown](#github-markdown)
    - [Reduce HTML elements in Markdown](#reduce-html-elements-in-markdown)
    - [Beautify and Markdown syntax](#beautify-and-markdown-syntax)
    - [Space after HTML element for markdown syntax](#space-after-html-element-for-markdown-syntax)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

# Markdown

[Markdown Cheat Sheet \| Markdown
Guide](https://www.markdownguide.org/cheat-sheet/)

### Dropdowns

```markdown
<details>
  <summary>Topic</summary>
  This text will be hidden.
</details>
```

### Table of content TOC

```markdown
Table of Contents
=================
  * [Topic](#class-name)
  <a href="class-name">Topic</a>
```

### Empty line break

```html
<!--sometimes an empty line break is required, so <br/> does not affect other syntax/elements in markdown-->
<br/>
<br/>
```

### Italic/ bold/ header

```markdown
<!--italic-->*Hello*
<!--bold-->**Hello**
<!--h3-->### Hello ###
```

### Making a code fence

````markdown
    ```html/css/markdown
      <!--insert code here-->
    ```
````

### Adding a shield.io badge

![shields.io](https://img.shields.io/static/v1?label=shields.io&message=badge&color=<color>&logo=Shields.io "fig:")  
[GitHub: How to add Shields \| Easy, visible info on your projects -
YouTube](https://www.youtube.com/watch?v=Dl-ekLb4quE&ab_channel=TroubleChute)  
[Shields.io: Quality metadata badges for open source
projects](https://shields.io/#your-badge)

Study the web link address carefully, input in place of `<input>` and
remove the `<` and `>` as well. Select the categories in the shields.io website
for interactive, dynamic badges linked to GitHub

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
Click on the categories, e.g. activity, version is the release version
tag e.g. `v1.0.0`, shield.io will automatically check if the version
exist or not.

### Transfer Typora TOC onto GitHub README.md

GitHub markdown uses **pandoc** markdown which differs from Typora
markdown. To turn the **Typora** markdown table of content TOC into
functional TOC in GitHub, we need to export the Typora file as
**Markdown (other spec)**.

1 - Go to **File > Preferences > Export**  
2 - Add export type as **Markdown (other spec) > variant:
GitHub-flavored markdown**  
3 - Install **pandoc** as instructed  
4 - Restart **PC? or Typora**  
5 - Export your **Typora** file: **File > Export > Markdown (other
spec)**  
6 - Your new file should have TOC that works in GitHub README.md/ GitHub
markdown

### GitHub markdown

**Create TOC in markdown File** - [GitHub TOC Generator](https://ecotrust-canada.github.io/markdown-toc/) by ecotrust-canada  
// Special characters such as `` or ** or : will invalidate the TOC link, as TOC generator turn it into `-` character. For example:

```markdown
[**Atom**](#--atom--) <!--invalid TOC link due to `**` special characters, conversion into `--` characters-->
```

### Reduce HTML elements in Markdown

When possible, avoid using HTML elements in Markdown, e.g. links, italics, bold. Focus on using Markdown syntax.

### Beautify and Markdown syntax

Beware that **Beautify** may affect some Markdown syntax. Use with caution in Markdown.

### Space after HTML element for markdown syntax

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