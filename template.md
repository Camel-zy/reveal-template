---
title: reveal模板
separator: <!--s-->
verticalSeparator: <!--v-->
css: theme.css
highlightTheme: github
revealOptions:
  transition: 'slide'
  transitionSpeed: 'fast'
  center: false
  slideNumber: c/t
---

<div class="center">
<div style="width: 100%">

<img src="cslogo.png">

# reveal模板

<hr />

Author

</div> 
</div> 

<!--s-->

# 一级标题

> 一句引用

一些文字

1. 第一点

2. 第二点

Note: 演讲者笔记

<!--v-->

## 二级标题

一些**代码**

```c[1|2-5]
#include <stdio.h>
int main() {
    printf("Hello World!");
    p->next = NULL;
    return 0;
}
```

<!--v-->

## 二级标题

### 三级标题

一些文字

- list
- list
  - list2

<!--v-->

## 表格

表格

| 项目 | 价格 | 数量 |
| :---- | :----: | ----: |
| 计算机 | 1600 | 5 |
| 手机 | 12 | 12 |
| 管线 | 1 | 234 |


<!--s-->

# 第三页

<!--v-->

## 二级标题

一些公式

$x^2+y^2=z^2$

<!--v-->

## 一些动画

<p class="fragment">Fade in</p>
<p class="fragment fade-out">Fade out</p>
<p class="fragment highlight-red">Highlight red</p>
<p class="fragment fade-in-then-out">Fade in, then out</p>
<p class="fragment fade-up">Slide up while fading in</p>

<!--v-->

## 超链接

<a href="#/0">Back to the first</a>


