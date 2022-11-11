# GitHub 使用遇到问题处理集合

在使用Github过程遇到各种问题，让后我们各种百度，现将已处理的问题归类总结分享下

### 1、readme.md无法显示图片

**问题现象**

![image-20221111165452008](../images/github-handle/image-20221111165452008.png)

**解决方案**

#### 1.1 图片的引入方式

1.1.1 网络资源图片引入方式

> ![]()  //[]中可选填图片文字说明,()*填写图片的url地址

1.1.2 git仓库图片引入方式

> ![](https://github.com/仓库名/项目名/blob/master/image/img.png)

**原因：如果你的README文件内显示图片的路径是正确的，那么很有可能是因为DNS被污染了所以导致显示不正常，即无法访问存放github图片素材的raw.githubusercontent.com站点**

以win10为例，将`C:\Windows\System32\drivers\etc\hosts`文件拷贝到桌面（因为该文件是在C盘如果你不拷贝出来是无法进行修改的），打开该文件添加两行

> 199.232.68.133 raw.githubusercontent.com
> 199.232.68.133 githubusercontent.com

打开命令行，输入：

>  ipconfig /flushdns

### 2、

