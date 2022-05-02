# runeflex

## Image

![runeflex command image](./runeflex.png)

## Required

runewidth command is required.  
runewidth "string" is return fixed width of the character "string".

I use [GitHub - mattn/go-runewidth: wcwidth for golang](https://github.com/mattn/go-runewidth) function as command line tool.  
See installation at <https://github.com/kis9a/go-runewidth#fork>

## Installation

```
sudo curl -s https://raw.githubusercontent.com/kis9a/runeflex/main/runeflex >/usr/local/bin/runeflex
chmod +x /usr/local/bin/runeflex
```

## Usage

```
USAGE:
  runeflex [options] [argument] [file1] [file...]

OPTIONS:
  -h, --help: show help
  -t, --test: test: runeflex_test
  -b, --border: border char of flexbox
  -g, --gap: gap space of flexbox
  -m, --margin: margin size
  -mx, --margin-x: horizontal margin size
  -my, --margin-y: vertical margin size
  -p, --padding: padding size
  -px, --padding-x: horizontal padding size
  -py, --padding-y: vertical padding size
```

### vim

Install runeflexrn

```
:'<,'>!runeflexrn -mx 4 -py 2 -b ab
```

## Devtools

**Style guide**

> Indentation
> Indent 2 spaces. No tabs. Use blank lines between blocks to improve readability. Indentation is two spaces. Whatever you do, don’t use tabs. For existing files, stay faithful to the existing indentation.
> <https://google.github.io/styleguide/shellguide.html>

Linter: [GitHub - koalaman/shellcheck](https://github.com/koalaman/shellcheck)  
Formatter: [GitHub - mvdan/sh](https://github.com/mvdan/sh)
