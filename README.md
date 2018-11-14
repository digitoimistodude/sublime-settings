# Settings for Sublime Text 3

This repository contains all the important Sublime Settings for collaborating with [Digitoimisto Dude Oy](https://www.dude.fi/). Copy, edit or overwrite desired files to your to `Packages/User/` (full path on macOS: `~/Library/Application Support/Sublime Text 3/Packages/User/`.

![Screenshot](https://i.imgur.com/JxENQnW.png)

## Contents

1. [Settings](https://github.com/digitoimistodude/sublime-settings/tree/master/settings) - Core settings
2. [Snippets](https://github.com/digitoimistodude/sublime-settings/tree/master/snippets) - Easy snippets via Tab completion, currently active for SCSS: `jeet`, `cover`, `block`, `media`, `stack`, `mobile`
3. [Keymaps](https://github.com/digitoimistodude/sublime-settings/tree/master/keymaps) - Common key combinations for macOS
4. [Linters](https://github.com/digitoimistodude/sublime-settings/tree/master/linters) - Error reporting settings for PHP and SCSS
5. [Themes](https://github.com/digitoimistodude/sublime-settings/tree/master/themes) - Custom themes for Sublime Text 3. **Note:** copy `tasks-markdown.hidden-tmTheme` to `Packages/` root directory

## Setting up

1. Copy all files from directories above to your `Packages/User/` folder.
2. Install **Package Control** ([Installation instructions](https://packagecontrol.io/installation))
2. Set up packages (below)

## List of packages

We try to keep this list as up to date as possible.

1. [All Autocomplete](#all-autocomplete)
2. [BracketHighlighter](#brackethighlighter)
3. [Color Highlight](#color-highlight)
4. [EditorConfig](#editorconfig)
5. [FileHeader](#fileheader)
6. [Generic Config](#generic-config)
7. [GitGutter](#gitgutter)
8. [JavaScript Next - ES6 Syntax](#javascript-next-es6-syntax)
9. [MarkdownEditing](#markdownediting)
10. [nginx](#nginx)
11. [PlainTasks](#plaintasks)
12. [ProjectManager](#projectmanager)
13. [Status Bar File Size](#status-bar-file-size)
14. [Stylefmt](#stylefmt)
15. [SublimeCodeIntel](#sublimecodeintel)
16. [SublimeLinter](#sublimelinter)
17. [SublimeLinter-scss-lint](#sublimeLinter-scss-lint)
18. [SublimeLinter-phpcs](#sublimeLinter-phpcs)
19. [SVGO](#svgo)
20. [Syntax-highlighting-for-Sass-legacy](#syntax-highlighting-for-sass-legacy)
21. [Theme - Spacegray](#theme-spacegray)

## Packages

Press **Cmd + Shift + P**, type **Package Control: Install Package** (or just "install") and install following. If there's no "Setting up", only thing you need to do is install package and that's it.

### [All Autocomplete](https://github.com/alienhard/SublimeAllAutocomplete)

**Why we use it:** This package extends Sublime autocompletion to find matches in all open files of the current window.

### [BracketHighlighter](https://github.com/facelessuser/BracketHighlighter)

**Why we use it:** Bracket Highlighter matches a variety of brackets such as: `[]`, `()`, `{}`, `""`, `''`, `<tag></tag>`, and even custom brackets in Sublime Text 3. This helps to see easier where code starts and ends.

### [Color Highlight](https://github.com/Kronuz/ColorHighlight)

**Why we use it:** Shows color codes (like "#ffffff", 0xffffff "rgb(255, 255, 255)", "white", hsl(0, 0%, 100%), etc.) with their real color as the background and/or gutter icons. Sometimes it's hard to say which color is which from just color code only.

### [EditorConfig](https://github.com/sindresorhus/editorconfig-sublime)

**Why we use it:** [EditorConfig](http://editorconfig.org) helps developers maintain consistent coding styles between different editors. When your `.editorconfig` file is in place in the project, every time you save you get indents and whitespaces removed etc. You will get .editorconfig file automatically if you use [dudestack](https://github.com/digitoimistodude/dudestack) or [air-light](https://github.com/digitoimistodude/air-light), otherwise get it [here](https://github.com/digitoimistodude/dudestack/blob/master/.editorconfig).

### [FileHeader](https://github.com/shiyanhui/FileHeader)

**Why we use it:** FileHeader makes it easier to create new file with initial contents. It also can add new header to an existed file or directory. This ensures every developer knows who and when file has been edited, doesn't have to check out git commits all the time.

**Setting up:** Copy file `FileHeader.sublime-settings` (comes with all the settings with this repo) to your `Packages/User/`, edit your mac username in place to that file, then copy `fileheaderes` folder to your `Packages/User/` directory.

### [Generic Config](https://github.com/skozlovf/Sublime-GenericConfig)

**Why we use it:** Generic highlighting of the configuration files for Sublime Text 2 and Sublime Text 3. Mainly for sysadmins.

### [GitGutter](https://github.com/jisaacks/GitGutter)

**Why we use it:** This plugin helps us to see git diff directly in the editor gutter. That way we can see modified time and user each row of the file.

### [JavaScript Next - ES6 Syntax](https://github.com/Benvie/JavaScriptNext.tmLanguage)

**Why we use it:** Better JavaScript language definition for TextMate and SublimeText. This builds on the language files commonly used and adds more fine grained matching and also includes new features from ECMAScript 6 like modules, succinct methods, arrow functions, classes, generators, and accessors (ES5).

### [MarkdownEditing](https://github.com/SublimeText-Markdown/MarkdownEditing)

**Why we use it:** Markdown plugin for Sublime Text. Provides a decent Markdown color scheme (light and dark) with more robust syntax highlighting and useful Markdown editing features for Sublime Text. 3 flavors are supported: Standard Markdown, GitHub flavored Markdown, MultiMarkdown. Optional, only for people who use markdown in documentation.

### [nginx](https://github.com/brandonwamboldt/sublime-nginx)

**Why we use it:** Improved syntax support for Nginx configuration files. Only for sysadmins.

### [PlainTasks](https://github.com/aziz/PlainTasks)

**Why we use it:** An opinionated todo-list plugin for Sublime Text editor. We use this for temporary checklists that are not worth to add to our team todo or project manager. These can be todolists that are inside the project, Dropbox or other places and can be run, checked and saved to file after completion.

**Setting up**: Install and activate, but please see [Contents](#contents) part 5 in themes, you need to copy PlainTasks markdown theme to a different place.

### [ProjectManager](https://github.com/randy3k/ProjectManager)

**Why we use it:** Don't have any idea what `*.sublime-project` and `*.sublime-workspace` are doing? Forget where the project files are? Don't worry, Project Manager will help organizing the project files by putting them in a centralized location. (It is inspired by Atom's Project Manager, but Atom's Project Manager is inspired by the built-in Sublime Text Project Manager, so there is a circular reasoning here).

**Setting up**: Install and activate. Sublime keymap file you copied to your `Packages/User/` should already contain a keymap to open project, it's `Cmd + Shift + O` (`{ "keys": ["super+shift+o"], "command": "project_manager", "args": {"action": "new"}},`).

To start a new project, open folder with Sublime Text or `subl -n ~/Projects/projectname` command, then type `Cmd + Shift + P` and choose **Project Manager: Add New Project**.

### [Status Bar File Size](https://github.com/SublimeText/StatusBarFileSize)

**Why we use it:** Displays file size in the Sublime Text status bar. Where possible, the size is queried from the file system. If this information is not available -- e.g. for a buffer that was modified and not yet saved -- the file size is estimated from the buffer contents and chosen encoding.

### [Stylefmt](https://github.com/dmnsgn/sublime-stylefmt)

**Why we use it:** Stylefmt is a tool that automatically formats CSS according to stylelint rules. Although, this is currently overridden by our gulpfile.js that runs stylefmt automatically on save, see [devpackages/gulpfile.js](https://github.com/digitoimistodude/devpackages/blob/master/gulpfile.js#L21).

### [SublimeCodeIntel](https://github.com/SublimeCodeIntel/SublimeCodeIntel)

**Why we use it:** Provides full-featured code intelligence and smart autocomplete for Sublime Text.

### [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter)

**Why we use it:** Lints the code you write which means, it reports about warnings and errors you should correct. Helps you write better code.

**Setting up**: Make sure you have the latest [Settings](https://github.com/digitoimistodude/sublime-settings/tree/master/settings).

### [SublimeLinter-scss-lint](https://github.com/attenzione/SublimeLinter-scss-lint)

**Why we use it:** Checks errors for SCSS syntax, using scss-lint. Makes sure we use same standard and write good code.

**Setting up**: Go through [Installation instructions](https://github.com/attenzione/SublimeLinter-scss-lint#installation).

### [SublimeLinter-phpcs](https://github.com/SublimeLinter/SublimeLinter-phpcs)

**Why we use it:** This linter plugin for SublimeLinter provides an interface to phpcs. It will be used with files that have the "PHP", "HTML" and "HTML5" syntax. Makes sure we use same standard and write good code.

**Setting up**: Install [phpcs](https://github.com/squizlabs/PHP_CodeSniffer#installation) to your `~/Projects` directory. Clone [PHPCompatibility](https://github.com/PHPCompatibility/PHPCompatibility) folder and [WordPress-Coding-Standards](https://github.com/WordPress-Coding-Standards/WordPress-Coding-Standards) to your `~/Projects` directory as well as `wpcs`. For this to work with Dude's config, you should have three folders: `~/Projects/phpcs`, `~/Projects/wpcs` and `~/Projects/PHPCompatibility`.

### [SVGO](https://github.com/attenzione/SublimeLinter-scss-lint)

**Why we use it:** SVG Optimizer is a Nodejs-based tool for optimizing SVG vector graphics files. Easy to use by typing `Cmd + Shift + P` and `svgo + enter`.

### [Syntax-highlighting-for-Sass-legacy](https://github.com/ronilaukkarinen/Syntax-highlighting-for-Sass-legacy)

**Why we use it:** A Sublime Text 3 package for highlighting both Sass and SCSS syntax. Legacy version of [Syntax-highlighting-for-Sass](https://github.com/P233/Syntax-highlighting-for-Sass). Works better with our custom theme, colors also complicated pseudos and other oddities.

**Setting up**: Type `Cmd + Shift + P` and choose **Package Control: Add Repository**. Paste this: `https://github.com/ronilaukkarinen/Syntax-highlighting-for-Sass-legacy` and press enter. Then install normally by choosing "Syntax-highlighting-for-Sass-legacy".

### [Theme - Spacegray](https://github.com/kkga/spacegray)

**Why we use it:** A Hyperminimal UI Theme for Sublime Text. Easy on the eyes.
