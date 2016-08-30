# html  

##　html书写

### 行元素

> 行标签：没有宽高属性，可与其他元素在一行显示
> 例如:
> a - 锚点
> b - 粗体(不推荐)  strong - 粗体强调
> i - 斜体          em - 斜体 
> strike - 删除线   s   del
> u - 下划线
> br - 换行
> span - 常用内联容器，定义文本内区块

> font - 字体设定(不推荐)
> img - 图片

> input - 输入框
> label - 表格标签
> select - 项目选择
> small - 小字体文本

> sub - 上标
> sup - 下标
> textarea - 多行文本输入框


### 行元素

> 块元素：可以设置宽高，但独占一行.
> 例如：div,h1,h2,h3,h4,h5,h6,p,ul,
> hr - 水平分隔线


# phpcsm整站制作

## 安装phpcms
	1、phpstudy 软件安装（有安装环境是前提）
	2、phpcmsv9.zip解压
	   install_package  redeme
	   把instrall_package下面的所有东西拷贝到www目录下
	3、打开localhost/index.html，开始安装
	4、安装过程中，注意事项
	   第3步：全新安装 
	   第5步: 账号 root   密码 root     email: 1@2.com
	5、点击后台管理    用户名 phpcms   密码  phpcms
	6、安装成功
	7、访问
	   后台：localhost/admin.php
	   前台：localhost/index.php
 
##　什么是内容管理系统？

> 用来制作动态网站的一个系统。
> 针对phpcmsv9
> 把index.php公开给用户去访问
> index.php是一段程序
> 这段程序根据得到的参数决定把哪个页面发送给用户
> 这段程序会在web服务器上寻找html和脚本，图片，拼接起来之后发送给用户
> 同时会把数据库中的动态内容写入到这些html中	   


## 开始制作

### 打开文件所在位置

	html文件在哪里
	phpcms/templates/default/content/

	脚本和图片在哪里
	statics/css/dxm/index.css
	statics/js/dxm/index.js
	statics/image/dxm/

### 页面构成

	header.html + index.html + footer.html
	
	index.html页面中   开始写  {template "content","header"}
	index.html页面中   结尾写  {template "content","footer"}

### 引入

```html
 <link rel="stylesheet" type="text/css" href="{CSS_PATH}dxm/index.css">
 <script src="{JS_PATH}dxm/index.js"></script>
```

```html
	<div class="logo">
		<img src="{IMG_PATH}dxm/logo.png" alt="">
	</div>
```

```css
	.log{
		backgound-img:url('/statics/images/dxm/a.png')
	}
```

### important 
