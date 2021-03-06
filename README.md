# Copy Selection as Markdown

Copy title, URL, selection as Markdown

- [Install](#install)
- [Usage](#usage)
- [Settings](#settings)
  - [General](#general)
  - [Markdown Styles](#markdown-styles)
    - [Heading style](#heading-style)
    - [Bullet list marker](#bullet-list-marker)
    - [Code block style](#code-block-style)
    - [Fence](#fence)
    - [Em](#em)
    - [Strong](#strong)
    - [Link style](#link-style)
    - [Link reference style](#link-reference-style)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Install

Go to [Add-ons for Firefox](https://addons.mozilla.org/en-US/firefox/addon/copy-selection-as-markdown/) and install.

## Usage

Right click and select:

- when part of the page is selected: **Copy Selection as Markdown**
- when user context-clicks in the page: **Copy Title and URL as Markdown**

## Settings

The add-on have multiple configuration to suit your setup as follows. Set your preference by:

1. Click the menu button ![](images/menu.svg) and choose ![](images/extensionGeneric-16.svg) **Add-ons**. The Add-ons Manager tab will open
2. In the Add-ons Manager tab, select the **Extensions** panel
3. Find **Keyboard shortcuts**, or **Copy Selection as Markdown** and click **Preferences**
4. Hit **Save** button to apply changes (no restart required)

### General

- Append quote (<code>&gt;</code>) to selection
- Include link to source web page in the beginning of copied text
- Enable experimental MathJax support
- Enable <a href="https://github.github.com/gfm/">GitHub Flavored Markdown</a> (strikethrough, tables, and taskListItems) support

### Markdown Styles

#### Heading style

- Setext
  ```
  Heading 1
  =========
  Heading 2
  ---------
  ```
- ATX (default)
  ```
  # Heading 1
  ## Heading 2
  ```

#### Bullet list marker

- Minus (`-`) (default)
  ```
  - one
  - two
  - three
  ```
- Plus (`+`)
  ```
  + one
  + two
  + three
  ```
- Asterisk (`*`)
  ```
  * one
  * two
  * three
  ```

#### Code block style

- Indented (default)
  ```
          let code = "indented";
  ```
- Fenced
  ````
      ```
      code = "fenced";
      ```
  ````

#### Fence

- Backticks (```) (default)
  ````
      ```
      let code = "fenced";
      ```
  ````
- Tildes (`~`)
  ```
      ~~~
      let code = "fenced";
      ~~~
  ```

#### Em

- Underline (`_`) (default)
  ```
  _Em_
  ```
- Asterisk (`*`)
  ```
  *Em*
  ```

#### Strong

- Underlines (`__`)
  ```
  __Strong__
  ```
- Asterisks (`*`) (default)
  ```
  **Strong**
  ```

#### Link style

- Inlined (default)
  ```
  [Inlined](https://example.com)
  ```
- Referenced
  ```
  [Referenced][1]<br/>
  [1]: https://example.com
  ```

#### Link reference style

- Reference (default)

  ```
  [Reference][1]

  [1]: https://example.com
  ```

- Collapsed

  ```
  [Reference with collapsed style][]

  [Reference with collapsed style]: https://example.com
  ```

- Shortcut

  ```
  [Reference with shortcut style]

  [reference with shortcut style]: https://example.com
  ```

## Contributing

Please read [CONTRIBUTING](CONTRIBUTING.md) for details.

## License

This extension is released under the MIT License. See [LICENSE](LICENSE) for details.

## Acknowledgements

- [Turndown](https://github.com/domchristie/turndown), which does all the heavy lifting from HTML to markdown
- [Octicons](https://octicons.github.com/) [clippy](https://octicons.github.com/icon/clippy/)
