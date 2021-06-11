# CodeMirror PCRE mode

This is a [CodeMirror](https://codemirror.net/) mode that brings syntax highlighting for [Perl Compatible Regular Expressions (PCRE)](https://www.pcre.org/).

## How to use
### Basic use
Load `pcre.js` and `pcre.css` at adequate locations in your HTML structure.
Mention `mode: 'pcre'` when creating your CodeMirror instance.

### Configuration
codemirror-mode-pcre supports extended mode (`x` flag) and actually enables it by default. This can be turned off by passing `extended: false` when creating the CodeMirror instance.

### Theming
This mode does not leverage CodeMirror's default tokens (they are not exactly fitted for regular expressions). Consequently, if you use a theme other than the default one, you will likely want to write your own `pcre.css` file.

## Non-features
codemirror-mode-pcre does **not** offer:
- completion (e.g. suggesting POSIX class names or script names for `\p` and `\P`);
- tooltips reflecting what the various parts of an expression actually mean;
- nested mode, i.e. the ability to highlight regular expressions as part of another mode;
- support for fancy module loaders.

Those may come in the future though.

## License
Like the PCRE library, this mode is released under the 3-clause BSD license.

