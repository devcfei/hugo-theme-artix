---
title: "Site Basic"
date: 2021-05-27T09:01:20+08:00
#draft: true
---


# Site basic configuration

- Logo
- Brand
- Sub-brand
- Multiple level menus
- Search
- Legal infomation
- Code highlight
- Table of contents


## Logo, brand and sub-brand

The logo should be configured by replace the `static/images/favicon.png`. The brand and sub-branded can be configured by the `config.toml`. The sub-brand is optional.

```toml
[params]
brand = "Artix"     # Brand of Site
subbrand = "Docs"   # Sub-Brand of Site, optional
```

## Code highlight


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
