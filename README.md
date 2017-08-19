# 前端一些网页的模仿与练习

## Search New Tab 
模仿FireFox自定义New Tab页
![Image text](https://raw.githubusercontent.com/wingofthestar/Web-front-end-Learning/master/Search_New_Tab.png)

## Baidu Tab
模范Baidu Tab页
![Image text](https://github.com/wingofthestar/Web-front-end-Learning/blob/master/Baidu_Tab.png?raw=true)

说明：并没有严格的仿照Baidu的网页来，关键是上手练习，Search New Tab页的搜索界面是用全部div布局的，问题比较少，这里尝试用span元素
转换为inline-block布局出现的问题有:
* inline-block元素之间有空白如何去除(这里我采用的事magrin负值，搜索一下有很多解决方案)
* input框和button无法对齐（vertical-align: 调整input元素的基线）
* 浏览器中查看div盒模型发现input的边框是向里增大的，而button的边框却是向外增大的，查阅发现chrome浏览器中默认的input是content-box
模型 而 button却是border-box模型（通过CSS3 box-sizing 属性手动将button调整为content-box模型）
![Image text](https://github.com/wingofthestar/Web-front-end-Learning/blob/master/img/%E7%9B%92%E6%A8%A1%E5%9E%8B.png?raw=true)
