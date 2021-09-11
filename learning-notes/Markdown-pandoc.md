<div id="toc">

[Markdown](#markdown)  
  [Dropdowns](#dropdowns)  
  [Table of content TOC](#table-of-content-toc)  
  [Empty line break `<br/>`](#empty-line-break-br)  
  [Italic/ bold/ header](#italic-bold-header)  
  [Making a code fence](#making-a-code-fence)  
  [Adding a shield.io badge ](#adding-a-shieldio-badge)

</div>

# Markdown

[Markdown Cheat Sheet \| Markdown
Guide](https://www.markdownguide.org/cheat-sheet/)

### Dropdowns

``` markdown
<details>
	<summary>Topic</summary>
	This text will be hidden.
</details>
```

### Table of content TOC

``` markdown
Table of Contents
=================
  * [Topic](#class-name)
  <a href="class-name">Topic</a>
```

### Empty line break `<br/>`

``` html
<!--sometimes an empty line break is required, so <br/> does not affect other syntax/elements in markdown-->
<br/>
<br/>
```

### Italic/ bold/ header

``` markdown
<!--italic-->*Hello*
<!--bold-->**Hello**
<!--h3-->### Hello ###
```

### Making a code fence

```` markdown
```html/css/markdown
	<!--insert code here-->
```
````

### Adding a shield.io badge 

![](https://img.shields.io/static/v1?label=shields.io&message=badge&color=<color>&logo=Shields.io "fig:")  
[GitHub: How to add Shields \| Easy, visible info on your projects -
YouTube](https://www.youtube.com/watch?v=Dl-ekLb4quE&ab_channel=TroubleChute)  
[Shields.io: Quality metadata badges for open source
projects](https://shields.io/#your-badge)

Study the web link address carefully, input in place of <input> and
remove the \<\> as well. Select the categories in the shields.io website
for interactive, dynamic badges linked to GitHub

**Markdown:**

``` markdown
<!--https://shields.io/--> <!--Markdown-->
![name](https://img.shields.io/static/v1?label=<label>&message=<message>&color=<color>&logo=<name>)
```

**HTML:**

``` html
<!--https://shields.io/--> <!--HTML-->
<img alt="alt-text" src="https://img.shields.io/static/v1?label=<label>&message=<message>&color=<color>&logo=<name>">

<!--to make the badge into a link using anchor href-->
<a href="https://atom.io/" target="_blank"><img alt="Atom shields.io" src="https://img.shields.io/static/v1?label=Atom&message=editor&color=teal&logo=Atom"></a>
```

**Activity: version**  
Click on the categories, e.g. activity, version is the release version
tag e.g. `v1.0.0`, shield.io will automatically check if the version
exist or not.
