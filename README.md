# remote-debugging
# 移动端远程调试

### http://blog.csdn.net/freshlover/article/details/42528643

## 准备工作
- 开发环境安卓桌面版Chrome32+
- 一条USB数据线，连接电脑与移动设备，安装相应机型的USB驱动。驱动程序下载地址：http://developer.android.com/tools/extras/oem-usb.html
- 如果是调试网页，移动设备需要安装**Chrome forAndroid** ，且安卓系统须为Android 4.0+

## 一些设置
第一步：首先在移动设备上开启USB调试模式。方法：

● Android 3.2+，打开设置 – 应用程序 – 开发，在“USB调试”处打钩选上

● Android 4.0~ Android 4.1 ，打开设置-开发者选项-进入在“USB调试”处打钩选上。

● Android 4.2+，打开设置-关于手机-手机配置信息-连点“版本号”7次，返回上层就可以看到“开发者选项”显示出来了，在“USB调试”处打钩选上。

![image](D:ss1-1.png)

![image](D:ss1-2.png)


第二步：用USB数据线连接设备，驱动装好连接成功后，你可能会在设备上看到一个弹框请求允许使用这台计算机通过usb调试。勾选后点击“确定”。

第三步：启动**Chrome forAndroid**，输入要调试页面的页面。

第四步：直接在浏览器地址栏输入chrome://inspect 或者about:inspect
打开后DevTools后，确保打钩选中Discover USB devices

![image](D:ss11-2.png)

第五步：点击inspect，打开Developer Tools。如下图：

![image](D:ss111-4.png)
![image](D:ss111-1.png)


## APP WebView调试
对于内嵌到App里的h5页面，远程调试方法也基本相同，只要打开app，进入到相应页面即可。



## 微信调试
微信调试因为涉及到JS-SDK调试，需要额外下载个**微信开发者工具**。操作同Chrome浏览器，

=> https://mp.weixin.qq.com/wiki/10/e5f772f4521da17fa0d7304f68b97d7e.html

微信开发者文档里的介绍很全，直接查看上面链接即可。


就是有一点需要注意下：因为只能调试自己绑定过的公众号，必须先公众号登录管理后台，绑定下。

![image](D:weChat-1.png)

绑定后，打开微信开发者工具，输入网址即可。最终的调试界面，如下：

![image](D:weChat-2.png)

![image](D:weChat-3.png)

当然，也支持远程调试。使用方法甚至更简单，直接上图：
![image](D:weChat-4.png)
![image](D:weChat-5.png)
![image](D:weChat-6.png)


## Node调试
...







