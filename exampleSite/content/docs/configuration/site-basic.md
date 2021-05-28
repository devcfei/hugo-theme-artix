---
title: "Site Basic"
date: 2021-05-27T09:01:20+08:00
weight: 1
#draft: true
---


# Site basic configuration

- Logo, brand and sub-brand
- Multiple level menu
- Search
- Legal infomation
- Code highlight
- Table of contents


## Logo, brand and sub-brand

The logo should be configured by replace the `static/images/favicon.png`. The brand and sub-branded can be configured by the `config.toml`. The sub-brand is optional.

**Example**
```toml
[params]
brand = "Artix"     # Brand of Site
subbrand = "Docs"   # Sub-Brand of Site, optional
```


## Multiple level menu

The multiple level menu should be configured by the global site setting in `config.toml`, up to 3 level supported.

```toml
#
# top menu shotcuts
#
[menu]
[[menu.shotcuts]]
name = "Home"
url = "/"
weight = 1

[[menu.shotcuts]]
name = "Getting Start"
url = "/tutorials/get-started"
weight = 2

[[menu.shotcuts]]
name = "Tutorials"
url = "/tutorials"
weight = 3

[[menu.shotcuts]]
name = "Docs"
url = "/docs"
weight = 4
identifier ="document"

[[menu.shotcuts]]
name = "About"
url = "/About"
weight = 5

#
# 2nd level menu
#
[[menu.shotcuts]]
parent = "document"
name = "Configuration"
url = "/docs/configuration"
weight = 1

[[menu.shotcuts]]
parent = "document"
name = "Markdown"
url = "/docs/markdown"
weight = 2
identifier ="markdown"


#
# 3rd
#
[[menu.shotcuts]]
parent = "markdown"
name = "Highlight"
url = "/docs/markdown/codehighlight"
weight = 1
```


## Code highlight

Code highlight is a hugo inbox feature, refers to [Hugo](https://gohugo.io/content-management/syntax-highlighting/#generate-syntax-highlighter-css)

```toml
[markup]
[markup.highlight]
codeFences = true
guessSyntax = false
hl_Lines = ""
lineNoStart = 1
lineNos = true
lineNumbersInTable = true
noClasses = true
style = "monokailight"
tabWidth = 4
```

**Change the code font size by CSS**
```css
.highlight pre{
    font-size: large;
}
```

## Table of contents

TOC is a hugo inbox feature, refers to [Hugo](https://gohugo.io/getting-started/configuration-markup#table-of-contents) for details


**Example**
```toml
[markup]
[markup.tableOfContents]
endLevel = 3
ordered = false
startLevel = 1
```
