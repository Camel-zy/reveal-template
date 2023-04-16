# reveal-template
A simple template for reveal slides

css模板由官方simple主题修改得来

由于前端知识较为欠缺，因此对主题的修改内容较少 能用就行（逃

# 使用方式
1. 安装 [reveal-md](https://github.com/webpro/reveal-md)
```bash
npm install -g reveal-md
```
2. 启动本地服务器，将指定的Markdown作为reveal.js演示文稿打开
```bash
reveal-md slides.md
```
3. 在浏览器中实时预览，修改Markdown将触发浏览器自动重新加载
```bash
reveal-md slides.md -w  # watch
```
4. 导出静态HTML文件
```bash
reveal-md slides.md --static _site
```
5. 导出pdf
    1. 使用Puppeteer生成pdf
    ```bash
    reveal-md slides.md --print slides.pdf
    ```
    但实测这样效果不好，会有诡异的排版和空白页

    2. 在浏览器地址栏后加上`?print-pdf`，然后打印为pdf（确保url中没有#等后缀）

5. 快捷键
- f: 全屏显示(按下Esc或f退出)
- s: 演讲者模式
- o: 总览视图
- v/.: 黑屏

# 编辑

1. 演讲者笔记
```markdown
Note: 以Note:开头的内容为演讲者笔记
```
2. 代码高亮
````markdown
需在语言后面加上方括号指定高亮的行
```c[1|2-5]
#include <stdio.h>
int main() {
    printf("Hello World!");
    return 0;
}
```
````
3. 淡入淡出等动画
详细查看[官方文档](https://revealjs.com/fragments/)
```html
<p class="fragment">Fade in</p>
<p class="fragment fade-out">Fade out</p>
<p class="fragment highlight-red">Highlight red</p>
<p class="fragment fade-in-then-out">Fade in, then out</p>
<p class="fragment fade-up">Slide up while fading in</p>
```