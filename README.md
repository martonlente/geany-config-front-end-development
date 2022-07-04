# Geany for front-end development (v0.2.0)

[Geany](https://github.com/geany/geany) is an open-source lightweight GUI text editor and IDE, that has been around since 2005.

Geany by default comes with limited support for front-end languages, but its configuration files options enable flexible custom improvements.

This repository is a light set of configuration files and opinionated conventions to streamline front-end development in Geany.

Geany for front-end development is based on the archived [geany-for-front-end-dev](https://github.com/trongthanh/geany-for-front-end-dev) repository by [@trongthanh](https://github.com/trongthanh), but made with a slightly different focus.

Geany for front-end development is under construction. :construction:

## Installation
Download Geany for front-end development, and copy the `geany` folder content to the Geany user config directory at `~/.config`:
```bash
cp -R geany/* ~/.config
```

## Usage
Study the `geany` folder structure's layout, and the configuration files.

```
.
├── filedefs
│   ├── filetypes.html
│   ├── filetypes.LESS.conf
│   └── filetypes.SCSS.conf
├── filetype_extensions.conf
├── snippets.conf
└── tags
    ├── jquery.js.tags
    ├── std.css.tags
    ├── std.js.tags
    ├── std.less.tags
    ├── std.scss.tags
    └── styles.js.tags
```

### Syntax highlighting

---
Geany syntax highlighting can be expanded with custom filetypes. Geany for front-end development adds basic syntax highlighting support currently for the following filetypes:
- `html.twig`
- `less`
- `scss`

### Autocompletion

---
Geany offers autocompletion for symbols, words, and snippets.

#### Symbols autocompletion

Geany autocompletion can be expanded with global tags files. Geany for front-end development adds autocompletion symbol support currently for the following languages:
- CSS
- LESS
- JavaScript
- JQuery
- SCSS

CSS, LESS and SCSS autocompletions are currently in sync with Geany's default CSS syntax highlighting support as of version 1.38. JavaScript and jQuery autocompletion support is ported from [geany-for-front-end-dev](https://github.com/trongthanh/geany-for-front-end-dev) repository, and needs to be updated.

#### Snippets autocompletion
Geany autocompletion can be expanded with user-definable snippets. Snippets are small strings which can be replaced or completed to a more complex string or code construct. The default key to start autocompletion is `TAB`. Geany for front-end development improves snippet support currently for the following languages:
- HTML

Improvements for JavaScript may be added in future.

### Preferences

---
#### Preferences conventions
I recommend changing the following default preferences:
- Editor | Features | Line wrapping | <checked>
- Editor | Features | Comment toggle marker | <empty>
- Editor | Indentation | Width: | 2
- Editor | Indentation | Type: | Spaces
- Editor | Completions | Autocomplete all words in document | <checked>
- Editor | Completions | Characters to type for autocompletion: | 2

Note that Auto-close quotes and brackets currently doesn't work within symbols, so I suggest enabling `autoclose` Geany plugin instead.

#### Themes
[Geany-themes](https://github.com/geany/geany-themes) add colour schemes for Geany. I recommend installing `geany-themes` with your package manager, and then choosing your preferred theme.

I currently recommend Monokai.

#### Plugins
[Geany plugins](https://github.com/geany/geany-plugins) extend the functionality of Geany. I recommend installing all `geany-plugins-*` with your package manager, and then enabling your preferred plugins. Plugins add a lot of useful features common in popular editors like Atom and Visual Studio Code, and improve the UX in lots of areas.

I currently recommend enabling the following plugins:
- `addons`
- `autoclose`
- `automark`
- `filebrowser`
- `git-changebar`
- `markdown`
- `overview`
- `projectorganizer`
- `spellcheck`
- `splitwindow`

Note that some plugins' features overlap.

## Contributing
Pull requests are not yet welcome. For support requests, please open an issue first to discuss what you would like to change.

## License
[Apache 2.0](https://github.com/martonlente/geany-for-front-end-development/blob/main/LICENSE)
