# 简介 #
该RotateLayout的功能，主要是仿照酷狗ios版本的旋转界面功能来实现，目前主要实现了左旋转和右旋转，该功能主要是在我的乐乐音乐播放器里面使用，其项目地址如下：
https://github.com/zhangliangming/HappyPlayer5.git 。

# 日志 #

## v2.5 ##
1.minSdkVersion 修改为19

## v2.2 ##
1.添加混淆
2.修复

## v1.8 ##
1. 添加了旋转角度回调事件
2. 添加了旋转角度的旋转中心坐标

## v1.0 ##
1. 实现左旋转和右旋转关闭界面功能

# 截图 #

![](https://i.imgur.com/uDlWQoK.png)

# Gradle #
1.root build.gradle

	`allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}`
	
2.app build.gradle

`dependencies {
	         compile 'com.github.zhangliangming:RotateLayout:v2.6'
	}`

# 混淆注意 #
-keep class com.zlm.libs.widget.** { *; }

# 调用Demo #
链接: https://pan.baidu.com/s/1pMXX4lP 密码: y6p7

# 第一种调用用法 #
1. AndroidManifest.xml

![](https://i.imgur.com/81SVixF.png)

1. styles.xml（activity的主题）

![](https://i.imgur.com/KVD6KQP.png)

2. activity.xml

![](https://i.imgur.com/iamc48K.png)

3. test_com.xml

内容布局，普通布局即可

4. java调用
- 初始化

![](https://i.imgur.com/2wZsCOe.png)

- activity返回事

![](https://i.imgur.com/KHZmsd9.png)

# 第二种调用用法 #

用法具体和第一种差不多

![](https://i.imgur.com/Z5Kq9Tc.png)

![](https://i.imgur.com/KHZmsd9.png)

# API #
- addIgnoreHorizontalView：添加水平方向不拦截的view
- setContentView：默认是添加LinearLayout布局的view，contentViewType有两种：CONTENTVIEWTYPE_LINEARLAYOUT（LinearLayout类型） / CONTENTVIEWTYPE_RELATIVELAYOUT（RelativeLayout类型）
- setDragType：设置右旋转关闭（LEFT_TO_RIGHT）/左旋转关闭（RIGHT_TO_LEFT）/全部
- RotateLayoutListener：需要在view关闭时，关闭activity时使用


# 捐赠 #
如果该项目对您有所帮助，欢迎您的赞赏

- 微信

![](https://i.imgur.com/e3hERHh.png)

- 支付宝

![](https://i.imgur.com/29AcEPA.png)