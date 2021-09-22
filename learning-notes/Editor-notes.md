# Editor notes

Some helpful tips and extensions for editors for personal reference.

Table of content

- [Editor notes](#editor-notes)
  - [Font-family](#font-family)
  - [VS-Code](#vs-code)
    - [Extensions](#extensions)
    - [VSC Settings](#vsc-settings)
    - [Markdown Lint](#markdown-lint)
    - [Clone a Repository to VS Code](#clone-a-repository-to-vs-code)
  - [Atom](#atom)
    - [Packages](#packages)
    - [Settings](#settings)
    - [Linter-node-markdownlint by josa42 Configuration](#linter-node-markdownlint-by-josa42-configuration)
    - [Disabled - Mardownlint by leonelgalan Configuration](#disabled---mardownlint-by-leonelgalan-configuration)
  - [Linter rules](#linter-rules)
  - [GitHub Markdown](#github-markdown)
    - [Transfer Typora TOC onto GitHub README.md](#transfer-typora-toc-onto-github-readmemd)
    - [GitHub Markdown TOC](#github-markdown-toc)
    - [GitHub page customisation](#github-page-customisation)
    - [GitHub markdown relative links](#github-markdown-relative-links)
    - [Beautify and Markdown syntax](#beautify-and-markdown-syntax)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## Font-family

```html
<!--useful fonts-->
font-family: Monaco, Consolas, "Ubuntu Mono", monospace, Menlo, "Helvetica Neue Light", "Helvetica Neue";
```

---

## VS-Code

### Extensions

[Atom One Dark Theme](https://marketplace.visualstudio.com/items?itemName=akamud.vscode-theme-onedark) by Mahmoud Ali  
[Markdown Preview GitHub Styling](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles) by Matt Bierner  
[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) by Ritwick Dey  
[HTML Preview](https://marketplace.visualstudio.com/items?itemName=tht13.html-preview-vscode) by Thomas Haakon Townsend  
[Beautify](https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify) by HookyQR  
[File-icons](https://marketplace.visualstudio.com/items?itemName=file-icons.file-icons) by file-icons  
[Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) by Yu Zhang  
[Markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) by David Anson  
[GitHub Pull Requests and Issues](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github) by GitHub  

Extensions are stored in the following location  
`DRIVE:\Users\%USERPROFILE%\.vscode\extensions`

### VSC Settings

Settings > Text Editor > Minimap > Editor > Minimap: Render Characters  
Settings > Editor: Font-family  
Settings > Editor: Code Lens Font-family  
Settings > SCM: Input Font Family  
Settings > Debug > Console: Font Family  
Settings > Terminal > Integrated: Font Family  

### Markdown Lint

Rules can be enabled, disabled, and customized by creating a JSON file
named `.markdownlint.jsonc` / `.markdownlint.json` or a YAML file named
`.markdownlint.yaml` / `.markdownlint.yml` or a JavaScript file named
`.markdownlint.js` in any directory of a project.  

The default rule configuration disables MD013/line-length because many
files include lines longer than the conventional 80 character limit:  

```json
{
    "MD013": false
}
```

### Clone a Repository to VS Code

1 - `Ctrl`+`Shift`+`P` > Open "Command Palette"  
2 - "Git: Clone"  
3 - Input: Provide repository URL  
4 - Select Folder for clone location  

Syncing will not work (pull, push) if the repo is cloned into another repo. See [Git clone into another git repo](https://stackoverflow.com/questions/10360342/git-clone-into-another-existing-git-repo)  

---

## Atom

### Packages

[Emmet](https://atom.io/packages/emmet) by emmetio  
[File Icons](https://atom.io/packages/file-icons) by file-icons  
[Atom Live Server](https://atom.io/packages/atom-live-server) by jas-chen  
[Todo](https://atom.io/packages/todo) by reergymerej  
[Minimap](https://atom.io/packages/minimap) by atom-minimap  
[Pigments](https://atom.io/packages/pigments) by abe33  
[Linter](https://atom.io/packages/linter) by steelbrain  
[Linter-jshint](https://atom.io/packages/linter-jshint) by AtomLinter  
[Linter-jscs](https://atom.io/packages/linter-jscs) by AtomLinter  
[Atom-beautify](https://atom.io/packages/atom-beautify) by Glavin001  
[Ask a stack](https://atom.io/packages/ask-stack) by Chris911  
[Highlight selected](https://atom.io/packages/highlight-selected) by richrace  
[Linter](https://atom.io/packages/linter) by steelbrain (see install instructions)  
[Linter-ui-default](https://atom.io/packages/linter-ui-default) by steelbrain  
[Linter-markdownlint](https://atom.io/packages/linter-markdownlint) by leonelgalan (see install instructions)  
[Linter-node-markdownlint](https://atom.io/packages/linter-node-markdownlint) by josa42 [Preferred]  
[Atom-ide-ui](https://atom.io/packages/atom-ide-ui) by facebook-atom [Preferred]  

### Settings

  Settings > Editor > Show Indent Guide  
  Settings > Editor > Zoom Font When Ctrl Scrolling  
  Settings > Keybindings > Keymap file add:  

  ```js
    'atom-text-editor':
    'f10': 'editor:toggle-soft-wrap'
  ```  

### Linter-node-markdownlint by josa42 Configuration

1 - Follow the install instructions (install packages)  

|No.|Packages|
|---|--------|
|1.|Linter|
|2.|Linter-node-markdownlint (by josa42)|
|3.|atom-ide-ui|

2 - A conflict message may appear in atom if you have other linter-ui - select which ui to disable  
3 - Go to `DRIVE:\Users\%USERPROFILE%\.atom\packages\linter-node-markdownlint` and find `.markdownlintrc` file  
4 - Copy `.markdownlintrc` file and paste it to the root folder of repository  
5 - !!DO NOT add `.json` or other file type suffix to the file, otherwise, the config will not work.  
6 - Configure Linter-node-markdownlint package in `.markdownlintrc` file by adding code. Example as follow:  

```json
{
  "MD004": false,
  "MD007": false
}
```

Also See [Documentation and Repository](https://github.com/josa42/atom-linter-node-markdownlint) for Linter-node-markdownlint

### Disabled - Mardownlint by leonelgalan Configuration

1 - Follow the install instructions, (install packages) 1. Linter, 2. Linter-ui-default, 3. Linter-markdownlint.  
2 - Add the following to `DRIVE:\Users\%USERPROFILE%\.atom\config.cson` (choose Config... in Atom menu)

```cson
'linter-markdownlint':
  executablePath: 'mdl'
  severity: 'error'
```

3 - Go to `DRIVE:\Users\%USERPROFILE%\.atom\packages\linter-markdownlint`, then copy the `.mdlrc` file (important!) and copy the `.style.rb` file  
4 - Paste the `.mdlrc` and `.style.rb` files onto the root folder of repository  
5 - You can now configure the Markdown Linter in the `.style.rb` file by adding codes. Example as below:

```rb
all
exclude_rule 'MD009'
exclude_rule 'MD033'
```

Also see [Documentation and Repository](https://github.com/leonelgalan/linter-markdownlint) for Linter-markdownlint

---

## Linter rules

See [Markdownlint GitHub](https://github.com/DavidAnson/markdownlint) by David Anson.  

---

## GitHub Markdown  

### Transfer Typora TOC onto GitHub README.md  

GitHub markdown uses **pandoc** markdown which differs from Typora markdown. To turn the **Typora** markdown table of content TOC into functional TOC in GitHub, we need to export the Typora file as **Markdown (other spec)**.  

  1 - Go to **File > Preferences > Export**  
  2 - Add export type as **Markdown (other spec) > variant: GitHub-flavored markdown**  
  3 - Install **pandoc** as instructed  
  4 - Restart **PC? or Typora**  
  5 - Export your **Typora** file: **File > Export > Markdown (other spec)**  
  6 - Your new file should have TOC that works in GitHub `README.md` or GitHub markdown  

### GitHub Markdown TOC

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
logo: assets/img/logo_3.png
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

### Beautify and Markdown syntax

Beware that **Beautify** may affect some Markdown syntax. Use with caution in Markdown.  
