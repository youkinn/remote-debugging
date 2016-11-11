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


![0_1478857298644_ss1-1.png](http://angular.angular-china.org/fe467d0d-3424-4e9d-a0e2-7ec77742c7ca.png)
[0_1478857311254_ss11-2.png](http://angular.angular-china.org/6fecd812-63c0-483a-aace-7d2d949a7ede.png)


第二步：用USB数据线连接设备，驱动装好连接成功后，你可能会在设备上看到一个弹框请求允许使用这台计算机通过usb调试。勾选后点击“确定”。

第三步：启动**Chrome forAndroid**，输入要调试页面的页面。

第四步：直接在浏览器地址栏输入chrome://inspect 或者about:inspect
打开后DevTools后，确保打钩选中Discover USB devices


![0_1478857311254_ss11-2.png](http://angular.angular-china.org/6fecd812-63c0-483a-aace-7d2d949a7ede.png)


第五步：点击inspect，打开Developer Tools。如下图：


![1_1478857311255_ss111-1.png](http://angular.angular-china.org/35ec8075-2617-4f17-848c-ba9d1485567c.png)

![0_1478857311254_ss11-2.png](http://angular.angular-china.org/6fecd812-63c0-483a-aace-7d2d949a7ede.png)


## APP WebView调试
对于内嵌到App里的h5页面，远程调试方法也基本相同，只要打开app，进入到相应页面即可。



## 微信远程调试
微信调试因为涉及到JS-SDK调试，需要额外下载个**微信开发者工具**。操作同Chrome浏览器，

=> https://mp.weixin.qq.com/wiki/10/e5f772f4521da17fa0d7304f68b97d7e.html

微信开发者文档里的介绍很全，直接查看上面链接即可。


就是有一点需要注意下：因为只能调试自己绑定过的公众号，必须先公众号登录管理后台，绑定下。

![1_1478857320683_weChat-1.png](http://angular.angular-china.org/97679fdc-1d53-4dac-b8b2-991e260eb5b6.png)

绑定后，打开微信开发者工具，输入网址即可。最终的调试界面，如下：

![0_1478857320683_ss111-4.png](http://angular.angular-china.org/ed99c560-c0b0-4280-9f46-42734de3395b.png)

![1_1478857328838_weChat-3.png](http://angular.angular-china.org/762e98c6-5c75-4656-96c4-dc1e4ede905e.png)

当然，也支持远程调试。使用方法甚至更简单，直接上图：
![0_1478857328838_weChat-2.png](http://angular.angular-china.org/0bdbefe9-cb52-4659-99b5-d631e4a41563.png)

![2_1478857337386_weChat-6.png](http://angular.angular-china.org/0d736ccb-40f5-4a9b-ac86-6c1f6ba98ee0.png)

![1_1478857337386_weChat-5.png](http://angular.angular-china.org/11642254-41bd-4a35-bf68-37deb08129d1.png)


## Node调试
...







