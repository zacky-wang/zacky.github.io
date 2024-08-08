---
title: "Hugo Even主题使用指导"
date: 2020-08-18T10:37:56+08:00
lastmod: 2020-08-18T10:37:56+08:00
draft: true
tags: ["Hugo", "even"]
categories: ["Hugo"]
author: "Jaswine"

weight: 10
contentCopyright: MIT
mathjax: true
autoCollapseToc: true

---

正确使用`hugo`中`even`主题

---

# 文件头部

# 文章体

## 锚点(Anchor)

- 用法:使用`[锚点名称](#section-id)`可以锚定本文中地方
- Example: [锚点•文章体](#文章体)
## 代码高亮

- 用法:使用  *_```java _* 包住代码块
- Example:
```java
public class Student{
    private String name;
    private int age;
}
```

# 插件

## shortcodes

### 注释

- 样式：

---

{{%/* admonition note "I'm title!" false */%}}

biu biu biu.

{{%/* admonition type="note" title="note" details="true" */%}}

biu biu biu.

{{%/* /admonition */%}}

{{%/* admonition example */%}}

Without title.

{{%/* /admonition */%}}

{{%/* /admonition */%}}


- 源代码:

```markdown
{{%/* admonition note "I'm title!" false */%}}
biu biu biu.

{{%/* admonition type="note" title="note" details="true" */%}}
biu biu biu.
{{%/* /admonition */%}}

{{%/* admonition example */%}}
Without title.
{{%/* /admonition */%}}

{{%/* /admonition */%}}
```


