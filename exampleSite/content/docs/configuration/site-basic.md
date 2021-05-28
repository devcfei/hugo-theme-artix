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

The multiple level menu should be configured by the global site setting in `config.toml` 

```toml
[[menu.shortcuts]]
name = "Home"
url = "/"
weight = 1

[[menu.shortcuts]]
name = "Getting Start"
url = "/tutorials/get-started"
weight = 2

[[menu.shortcuts]]
name = "Tutorials"
url = "/tutorials"
weight = 3

[[menu.shortcuts]]
name = "Docs"
url = "/docs"
weight = 4

[[menu.shortcuts]]
name = "About"
url = "/About"
weight = 5
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
