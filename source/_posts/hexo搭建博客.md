# Hexo搭建Github静态博客

## 1.下载安装Git

1.1 Git下载地址： https://gitforwindows.org/ 

1.1.1 淘宝镜像下载Git：https://registry.npmmirror.com/binary.html?path=git-for-windows/

1.2 安装步骤: **一路默认安装**

![image-20221110201927428](../images/hexo搭建博客/image-20221110201927428.png)



![image-20221110202051381](../images/hexo搭建博客/image-20221110202051381.png)



## 2.下载安装node.js

2.1 node.js下载地址：https://nodejs.org/en/

2.2 安装步骤：一路默认安装

![image-20221110202447665](../images/hexo搭建博客/image-20221110202447665.png)



![image-20221110202652186](../images/hexo搭建博客/image-20221110202652186.png)



## 3.安装Hexo

3.1 利用npm命令，使用Git Bash安装hexo

3.2 输入命令：npm install -g hexo

> $ npm install -g hexo

![image-20221110202905552](../images/hexo搭建博客/image-20221110202905552.png)



## 4.初始化Hexo

4.1 使用命令在F盘下创建blog博客目录

4.2 切换到blog目录创建hexo文件夹

> $ mkdir hexo

4.3 在Hexo文件夹下输入命令：hexo init （初始化hexo）

![image-20221110203122591](../images/hexo搭建博客/image-20221110203122591.png)



![image-20221110203643406](../images/hexo搭建博客/image-20221110203643406.png)



4.4 修改Hexo目录下的配置文件_config.yml,进行基础配置

![image-20221110203531407](../images/hexo搭建博客/image-20221110203531407.png)

4.5 hexo可用的主题浏览（https://hexo.io/themes/），选择自己喜欢的博客主题：例如使用（hexo-theme-matery）主题

在Hexo文件夹下Git Bash

输入命令：cd themes

输入命令: mkdir hexo-theme-matery

输入命令: cd hexo-theme-matery

输入命令：git clone https://github.com/blinkfox/hexo-theme-matery.git

![image-20221111102428428](../images/hexo搭建博客/image-20221111102428428.png)



注：如果localhost:4000浏览出现（原因是[hexo](https://so.csdn.net/so/search?q=hexo&spm=1001.2101.3001.7020)在5.0之后把swig给删除了需要自己手动安装）

**出现问题**

![img](https://img-blog.csdnimg.cn/d75aa3981183496aa03f112dc81ceab8.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBAQ0RMX0x1RmVp,size_20,color_FFFFFF,t_70,g_se,x_16)

**解决方法**

>npm i hexo-renderer-swig

![image-20221110212249043](../images/hexo搭建博客/image-20221110212249043.png)

4.6 修改配置文件：修改主题名称

![image-20221111102625823](../images/hexo搭建博客/image-20221111102625823.png)

4.6 本地浏览博客：

4.6.1 输入hexo clean & hexo g & hexo s 组合命令

> hexo clean & hexo g & hexo s



![image-20221111100545028](../images/hexo搭建博客/image-20221111100545028.png)





4.6.3 在浏览器输入：localhost:4000

![image-20221111102709270](../images/hexo搭建博客/image-20221111102709270.png)



## 5.部署到Github上

5.1 申请Github账号

5.2 创建一个新的仓库：

![image-20221111103244003](../images/hexo搭建博客/image-20221111103244003.png)

5.3 配置仓库地址：

![image-20221111103353086](../images/hexo搭建博客/image-20221111103353086.png)



5.4 安装hexo-deployer-git自动部署发布工具

> npm install hexo-deployer-git --save



![image-20221111103621929](../images/hexo搭建博客/image-20221111103621929.png)



5.5 发布到Github

> hexo clean && hexo g && hexo d

![image-20221111103809469](../images/hexo搭建博客/image-20221111103809469.png)



![image-20221111110008819](../images/hexo搭建博客/image-20221111110008819.png)

5.6 测试访问：https://kingvitor.github.io/

![image-20221111110039875](../images/hexo搭建博客/image-20221111110039875.png)



