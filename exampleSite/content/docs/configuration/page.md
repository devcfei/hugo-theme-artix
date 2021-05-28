---
title: "Page"
date: 2021-05-27T10:11:34+08:00
weight: 2
#draft: true
---

# Page configuration

Page can be configurated by **Front Matter** which is a setting set by YAML or TOML


- Page layout
- Markdown extention
- Single page

## Three colums layout page

By default the page is a three colums page, the main content is always show. The navigator, table of contents, and the breadcrumb bar are configurable.

**Example**

```yml
---
title: "Page" # Used by left navigation and a part of title of the window
date: 2021-05-27T10:11:34+08:00
#draft: true # false to take part for build, hugo default supported
layouts:
    - nav         # Enable left navigation 
    - toc         # Enable Right navigation 
    - breadcrumb  # Enable Breadcrumb navigation 
mdext:
    - mermaid    # For a page need render Mermaid
    - wavedrom   # For a page need render WaveDrom
    - katex      # For a page need render KaTeX
---
```


## Single page

Single page is a raw page without nav, toc and breadcrumb, usually the home page is a single page, to enable a single page, set the `layouttype` to `single`. 

**Example**
```yml
---
title: "Home"
date: 2021-05-24T20:53:35+08:00
layouttype: "single" # make single page
---
```





