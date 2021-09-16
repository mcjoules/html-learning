### Editor notes

Some helpful tips and extensions for editors for personal reference.

Table of content

- [Editor notes](#editor-notes)
- [Font-family](#font-family)
- [VS-Code](#vs-code)
  - [Extensions](#extensions)
- [Atom](#atom)
  - [Packages](#packages)
- [Typora/ GitHub Markdown](#typora-github-markdown)
  - [GitHub Markdown TOC](#github-markdown-toc)
  - [Beautify and Markdown syntax](#beautify-and-markdown-syntax)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

### Font-family

```html
font-family: Monaco, Consolas, Ubuntu Mono, monospace;
```

### VS-Code

#### Extensions

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

<details>
  <summary>Settings</summary>

Settings > Text Editor > Minimap > Editor > Minimap: Render Characters  
Settings > Editor: Font-family  
Settings > Editor: Code Lens Font-family  
Settings > SCM: Input Font Family  
Settings > Debug > Console: Font Family  
Settings > Terminal > Integrated: Font Family  
</details>

<details>
  <summary>Markdown Lint</summary>

Rules can be enabled, disabled, and customized by creating a JSON file named `.markdownlint.jsonc` / `.markdownlint.json` or a YAML file named `.markdownlint.yaml` / `.markdownlint.yml` or a JavaScript file named `.markdownlint.js` in any directory of a project.  

The default rule configuration disables MD013/line-length because many files include lines longer than the conventional 80 character limit:  

```json
{
    "MD013": false
}
```

</details>

<details>
  <summary>Clone a Repository to VS Code</summary>

1. `Ctrl`+`Shift`+`P` > Open "Command Palette"  
2. "Git: Clone"  
3. Input: Provide repository URL  
4. Select Folder for clone location  

!!Syncing will not work (push, pull) if the repo is cloned into another repo.  
See [Git clone into another git repo](https://stackoverflow.com/questions/10360342/git-clone-into-another-existing-git-repo)

</details>

### Atom

#### Packages

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

<details>
  <summary>Settings</summary>

  Settings > Editor > Show Indent Guide  
  Settings > Editor > Zoom Font When Ctrl Scrolling  
  Settings > Keybindings > Keymap file add:  

  ```js
    'atom-text-editor':
    'f10': 'editor:toggle-soft-wrap'
  ```  

</details>

### Typora/ GitHub Markdown

<details>
  <summary>Transfer Typora TOC onto GitHub README.md</summary>

  GitHub markdown uses **pandoc** markdown which differs from Typora markdown. To turn the **Typora** markdown table of
  content TOC into functional TOC in GitHub, we need to export the Typora file as **Markdown (other spec)**.

  1 - Go to **File > Preferences > Export**  
  2 - Add export type as **Markdown (other spec) > variant: GitHub-flavored markdown**  
  3 - Install **pandoc** as instructed  
  4 - Restart **PC? or Typora**  
  5 - Export your **Typora** file: **File > Export > Markdown (other spec)**  
  6 - Your new file should have TOC that works in GitHub README.md/ GitHub markdown  

</details>

#### GitHub Markdown TOC

**Create TOC in markdown File** - [GitHub TOC Generator](https://ecotrust-canada.github.io/markdown-toc/) by ecotrust-canada  
// Special characters such as `` or ** or : will invalidate the TOC link, as TOC generator turn it into `-` character. For example:

```markdown
[**Atom**](#--atom--) <!--invalid TOC link due to `**` special characters, conversion into `--` characters-->
```

#### Beautify and Markdown syntax

Beware that **Beautify** may affect some Markdown syntax. Use with caution in Markdown.  
