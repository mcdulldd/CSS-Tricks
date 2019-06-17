# 前言

##  关于项目
该项目是作为《CSS揭秘》的读书笔记，基于`docsify`的在线文档。

### 快速开始
* clone这个仓库：[https://github.com/mcdulldd/CSS-Tricks](https://github.com/mcdulldd/CSS-Tricks)
* 安装docsify：`npm install docsify-cli -g`,如果速度太慢可以自行百度`淘宝镜像`解决
* 在终端运行命令 docsify serve ./docs
* 在浏览器中打开[http://localhost:3000](http://localhost:3000)

## CSS编码技巧
```css
/* 某些值相互依赖时，可以通过代码体现出来 */
div {
  font-size: 20px;
  line-height: 30px;
}
/* 修改后 */
div {
  font-size: 125%;
  line-height: 1.5;
}
/* 合理使用简写 */

div {
  background: url(tr.png) no-repeat top right / 2em 2em,
              url(br.png) no-repeat bottom right / 2em 2em,
              url(bl.png) no-repeat bottom left / 2em 2em;
}
/* 修改后 */
div {
  background: url(tr.png) top right,
              url(br.png) bottom right,
              url(bl.png) bottom left;
  background-size: 2em 2em;
  background-repeat: no-repeat;          
}
```

?> 参考：[You-need-to-know-css](https://lhammer.cn/You-need-to-know-css/#/)