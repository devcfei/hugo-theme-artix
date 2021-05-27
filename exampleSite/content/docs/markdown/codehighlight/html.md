---
title: "Html"
date: 2021-05-27T10:00:57+08:00
#draft: true
---

# Html code highlight

## Syntax and demo


**The markdown**
```markdown
<section id="main">
  <div>
   <h1 id="title">{{ .Title }}</h1>
    {{ range .Pages }}
        {{ .Render "summary"}}
    {{ end }}
  </div>
</section>
```

**Rendered as follow**
```html
<section id="main">
  <div>
   <h1 id="title">{{ .Title }}</h1>
    {{ range .Pages }}
        {{ .Render "summary"}}
    {{ end }}
  </div>
</section>
```
