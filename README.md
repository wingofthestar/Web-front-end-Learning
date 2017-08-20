# 前端一些网页的模仿与练习

## Search New Tab 
模仿FireFox自定义New Tab页
![Image text](https://raw.githubusercontent.com/wingofthestar/Web-front-end-Learning/master/Search_New_Tab.png)

## Baidu Tab
模范Baidu Tab页
![Image text](https://github.com/wingofthestar/Web-front-end-Learning/blob/master/Baidu_Tab.png?raw=true)

说明：并没有严格的仿照Baidu的网页来，关键是上手练习，Search New Tab页的搜索界面是用全部div布局的，问题比较少，这里尝试用span元素
转换为inline-block布局出现的问题有:
* inline-block元素之间有空白如何去除(这里我采用的是magrin负值，搜索一下有很多解决方案)
* input框和button无法对齐（vertical-align: 调整input元素的基线）
* 浏览器中查看div盒模型发现input的边框是向里增大的，而button的边框却是向外增大的，查阅发现chrome浏览器中默认的input是content-box
模型 而 button却是border-box模型（通过CSS3 box-sizing 属性手动将button调整为content-box模型）
![Image text](https://github.com/wingofthestar/Web-front-end-Learning/blob/master/img/%E7%9B%92%E6%A8%A1%E5%9E%8B.png?raw=true)

采用了字体图标（https://github.com/FortAwesome/Font-Awesome ）按照文档直接引用即可。

## ZhiHuLoginTab
开始看了较多知乎网页的源码，尝试着跟着写，结果太复杂以至于，变成复制黏贴式，于是还是放弃，按照自己的方式去写
知识点有:
 * 结构，看html的源码是几乎看下去的，看看人家是怎么样组织DOM结构，至于CSS嘛，实在吃不消看。
 * 不定宽高的div块等的水平垂直居中，搜索一下有很多方法，这里采用用一个“ghost”伪元素（看不见的伪元素）和 inline-block / vertical
 -align 可以搞定居中
 * 背景图用了canvas-nest.js,看上去效果不错(https://github.com/hustcc/canvas-nest.js )
