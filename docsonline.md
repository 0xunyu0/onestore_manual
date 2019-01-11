在线文档实现
===========

>需要懂一些Markdown 语法 良好的写作风格

>如果你对HTML CSS JavaScript不熟悉 请不要随意删减index.html 文件内容

>有时候你需要清除一下浏览器缓存(ctrl+shift+delete → enter) 才可以刷新页面！！！

## 几个简单的步骤 
**1.1 注册一个腾讯云开发者平台账号**
* 腾讯云开发者平台 [GO](https://dev.tencent.com/)

**1.2 新建一个项目 如图**
![docs][1]

  [1]:https://docs.iolab.top/_media/docs.jpg
**1.3 上传几个文件**
* docs 文件 [GET](https://docs.iolab.top/_media/docs.zip)

请解压docs.zip文件后ctrl+A 全选后上传所有文件

！！！文件夹需要自建

代码很纯正 请放心食用 

**在项目列表里创建_images文件夹**

！！！当文件夹下不包含文件时 文件夹也会被自动删除

创建一个文件夹需要输入新文件名_media后/ 再创建一个文件 例如a.md（内容可以空） 最后 点击右下角提交到master分支即可

**1.4 开启Pages服务**

**在 Pages服务里 点击自己的访问地址**

![docs][2]
	
  [2]:https://docs.iolab.top/_media/pages.jpg

**1.5 大功告成**
![docs][3]

  [3]:https://docs.iolab.top/_media/allisok.png
**1.6 开始使用**

**1.6.1 自定义封面**
修改_coverpage.md文件

![docs][4]

  [4]:https://docs.iolab.top/_media/face.png
**1.6.2 自定义左侧边栏**
修改_sidebar.md文件
![docs][5]

  [5]:https://docs.iolab.top/_media/sidebar.png
   >编写的文件请以.md作为后缀名 

**1.6.3 修改index.html 文件**
修改时光精灵文档标题

![docs][6]

  [6]:https://docs.iolab.top/_media/indexchange.jpg
**1.7 查看更多**

**1.7.1 去掉右上角github 图标**
``` html
	打开index.html文件找到如下代码 删除即可
    repo: 'https://github.com/time-fairy/',
	
```
* 项目官网 [GO](https://docsify.js.org/#/)
* github [GO](https://github.com/docsifyjs/docsify/)
