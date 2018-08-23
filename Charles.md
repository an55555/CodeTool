### 激活

`Help -> Registe`

```text
Registered Name: https://zhile.io
License Key: 48891cf209c6d32bf4
```
### 与翻墙不能共存

实际使用中，如果只是为了抓取手机上请求，可以取消勾选 `Proxy -> Window Proxy`，这样不抓电脑上的请求，只抓取手机上的请求

### 安装证书

1. `Help -> SSL Proxying -> Install Charles Root Certificate`

![](http://upload-images.jianshu.io/upload_images/3150602-cec9c776fb0f4a45.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

2. 安装证书-> 本地计算机 -> 将所有的证书都放入下列存储 -> 选择“受信任的根证书颁发机构” -> 完成

### 抓取手上的网络请求

1. 需要确保电脑和手机能ping通。
2. 首先打开Charles的代理功能。具体在菜单栏上选择 `Proxy -> Proxy Settings`，输入代理端口：8888，并勾上“nable transparent HTTP proxying”选项
3. 在手机的网络连接中，将HTTP代理切换成手动，填上 Charles 运行所在的电脑的 IP，以及端口号 8888
4. 设置完毕在手机上打开任意程序，此时，可以看到 Charles弹出手机请求连接的确认窗口，点击 “Allow” 即可完成设置。

### 过滤

1. 在想过滤的网络请求上右击，选择 “Focus”，之后在 Filter 一栏勾选上 Focussed 一项

![avatar](https://images2017.cnblogs.com/blog/824413/201712/824413-20171220063028287-1764528838.png)

2. `proxy -> recording setting -> include` 再点击“Add”，在弹出的窗口中输入需要监控的协议，主机地址，端口号等信息，来添加一个项目
