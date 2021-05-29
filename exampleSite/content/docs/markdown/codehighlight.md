---
title: "Code Highlight"
date: 2021-05-27T10:00:53+08:00
weight: 6
#draft: true
---

# Code highlight

Code highlight is a hugo inbox feature, enable code highlight by configuration and customized highlight makeup


## C code highlight

### Syntax and demo


**The markdown**
```markdown
#include <stdio.h>
int main()
{
    printf("hello world!\n");
    return 0;
}
```

**Rendered as follow**
```c
#include <stdio.h>
int main()
{
    printf("hello world!\n");
    return 0;
}
```



## Html code highlight

### Syntax and demo


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
