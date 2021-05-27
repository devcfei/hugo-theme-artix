---
title: "Right TOC"
date: 2021-05-27T21:40:51+08:00
weight: 4

layouts:
  - toc

#draft: true
---

# Table of content in the right side

## Enable the TOC
To enable the TOC, the `toc` should be definded in `layouts`

```yml
layouts:
    - toc         # Enable left navigation 
```

`alwaysTOC` in `config.toml` enable all the TOC even `toc` is not set in `layouts`

```toml
[params]
alwaysTOC = true    # always have TOC for a page
```


## Setting of the TOC

TOC is an inbox feature in Hugo, the `config.toml` example

```toml
[markup.tableOfContents]
endLevel = 3            # levels to show, 3 by default
ordered = false         # order enabled, false by default
startLevel = 1          # start level, 2 by default
```

## Customize the TOC

To customize the TOC, change the default setting of `table, tr, th, td` in `static/css/style.css`  

```css
body #TableOfContents > ul {  
    padding-left: 0em;
    font-size: small;

}

body #TableOfContents > ul li { 
    padding-left: 1em;
    font-size:small;
}

```