---
title: "Page"
date: 2021-05-27T10:11:34+08:00
#draft: true
---

# Page configuration

Page can be configurated by **Front Matter** which is a setting set by YAML or TOML


- Page layout
- Markdown extention


**Example**

```yml
---
title: "Page" # Used by left navigation and a part of title of the window
date: 2021-05-27T10:11:34+08:00
draft: true # true to take part for build, hugo default supported
layout:
    - nav         # Enable left navigation 
    - toc         # Enable Right navigation 
    - breadcrumb  # Enable Breadcrumb navigation 
mdext:
    - mermaid    # For a page need render Mermaid
    - wavedrom   # For a page need render WaveDrom
    - katex      # For a page need render KaTeX
---
```


