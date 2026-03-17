**2025年11月26日更新。**

[点我获取更多免费v2ray账号](https://gitlab.com/zhifan999/fq/-/wikis/v2ray%E5%85%8D%E8%B4%B9%E8%B4%A6%E5%8F%B7) 

**一、Windows免费翻墙软件**

Windows v2rayN 客户端：[Github最新版下载](https://github.com/2dust/v2rayN/releases/latest) (下载带core的文件) [Github镜像下载](https://jgithub.xyz/2dust/v2rayN/releases/latest) (下载带core的文件)

第一步，按照地址下载v2rayN客户端，然后解压缩后打开应用：

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayn202500.png)

第二步，在任务栏中找到蓝色V图标，单击打开客户端界面，点击配置项

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayn202501.png)

复制节点一键导入链接后，选择“从剪贴板导入分享链接”即可把节点导入到软件中，可以批量导入。或者也可以通过扫描二维码或者手动填写节点信息。

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayn202504.png)

第三步，鼠标选中想用的节点，右键选择设置为活动服务器或者按回车，启用该节点。软件每次只能启用1个节点。

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayn202502.png)

第四步，在任务栏中右键v2rayN图标，选择“自动配置系统代理”，之后就可以通过浏览器翻墙了。

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayn202503.png)

如果路由选择“绕过大陆”，那么国内没有被封的网址就没有被代理。如果路由选择“全局”，那么所有的网址都会被代理。

**快速检测节点是否有效**

选中所有节点，选择“测试真链接”，如果延迟结果是“-1”，那么该节点不可用，反之节点可用。

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayn202505.png)

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayn202506.png)

***

**二、Mac免费翻墙软件**

Mac客户端1 v2rayN 7.15.7

**Apple M芯片-v2rayN-macos-arm64.dmg**

- [国外云盘下载](https://download.840899.xyz/v2rayN-macos-arm64.dmg)
- [Github下载](https://github.com/2dust/v2rayN/releases/download/7.15.7/v2rayN-macos-arm64.dmg)

**Intel芯片-v2rayN-macos-64.dmg**

- [国外云盘下载](https://download.840899.xyz/v2rayN-macos-64.dmg)
- [Github下载](https://github.com/2dust/v2rayN/releases/download/7.15.7/v2rayN-macos-64.dmg)

**注意：由于安装包没有签名，会提示应用已损坏；安装后需要运行**：xattr -cr /Applications/v2rayN.app 或者sudo xattr -d com.apple.quarantine /Applications/v2rayN.app

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayn202508.png)

**安装教程如下**：

根据自己Mac的芯片类型，选择下载Mac v2rayN 客户端下载文件：
v2rayN-macos-arm64.dmg或 v2rayN-macos-64.dmg

双击打开下载文件后，v2rayN Installer 窗口弹出。将v2rayN图标拖到Applications图标：

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202501.jpg)

如果屏幕弹出窗口：

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202502.jpg)

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202503.jpg)

在设置中找到v2rayN 路径：设置Settings – General – About – System Report，点开 System Report: 

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202512.jpg)

在 System Report 的左边找到Software，点开其中 Applications，右边往下滑找到 v2rayN 客户端，点开，复制它的位置 Location: /Applications/v2rayN.app：

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202505.jpg)

到应用夹Applications box搜索TERMINAL，找到后点开，输入强制启动命令：
xattr -cr / Applications/v2rayN.app, 回车后输入本电脑密码（输入密码时屏幕不显示任何东西），回车：

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202506.jpg)

到应用夹Applications 里找到v2rayN图标，双击打开，参考此网站Mac 启用第三方 APP 打开权限（允许“任何来源”），在“设置” -“私隐和安全性” - “安全性”中，选择“仍要打开“，然后打开v2rayN客户端。

从节点网站一键复制相应节点，黏贴到v2rayN 左上角 “配置” Configurations 中的 Import Share Links from clipboard (Ctrl+V)。可黏贴导入多个节点:

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202507.jpg)

在v2rayN 屏幕下方代理 Proxy选项中选 “Set system proxy”，在其隔壁右边V3选项中选 “V3-全局 (Global)”:

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202508.jpg)

右击已导入节点选择 “Set as active Configuration (Enter)”（或直接回车），选择后被选节点显示红色 “Active”图示，屏幕右上角v2rayN 图标变红色，此时应已连上：

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202509.jpg)

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/macv2rayn202510.jpg)

此时外网应连接上。

***

Mac客户端2 Hiddify 2.5.7 文件名称：Hiddify-MacOS.dmg

[下载地址1](https://download.979862.xyz/Hiddify-MacOS.dmg) [下载地址2](https://download.840899.xyz/Hiddify-MacOS.dmg) [下载地址3](https://download.186408.xyz/Hiddify-MacOS.dmg) [github最新版下载](https://github.com/hiddify/hiddify-app/releases)

MAC安装：

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/mac-002.jpg)

MAC启动：

⚠️【必读】如提示：无法打开“Hiddify”，看下图解决方案【按1、2、3、4 红字顺序操作】。

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/mac-001.png)

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/mac-003.jpg)

安装好后，点击+新的配置文件，找到v2ray节点的一键导入链接，复制链接，点击“剪贴板添加”。

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/mac-004.jpg)

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/mac-005.jpg)

[点我获取免费v2ray账号](https://gitlab.com/zhifan999/fq/-/wikis/v2ray%E5%85%8D%E8%B4%B9%E8%B4%A6%E5%8F%B7)

***

**三：Linux免费翻墙软件**

Linux客户端1：[v2rayN v7.15](https://github.com/2dust/v2rayN/releases/tag/7.15.7)

DEB包(Debian系) 使用 apt ./路径 安装

  **64位-v2rayN-linux-64.deb**
  - [国外云盘下载](https://download.840899.xyz/v2rayN-linux-64.deb) 
  - [Github下载](https://github.com/2dust/v2rayN/releases/download/7.15.7/v2rayN-linux-64.deb) 

  **Arm64-v2rayN-linux-arm64.deb**
  - [国外云盘下载](https://download.840899.xyz/v2rayN-linux-arm64.deb) 
  - [Github下载](https://github.com/2dust/v2rayN/releases/download/7.15.7/v2rayN-linux-arm64.deb)


RPM包(Redhat系) 使用 dnf ./路径 安装

  **Rhel-v2rayN-linux-rhel-arm64.rpm**
  - [国外云盘下载](https://download.840899.xyz/v2rayN-linux-rhel-arm64.rpm) 
  - [Github下载](https://github.com/2dust/v2rayN/releases/download/7.15.7/v2rayN-linux-rhel-arm64.rpm)

***

Linux客户端2：Hiddify-Linux-x64.AppImage v2.05

- [国外云盘下载](https://download.840899.xyz/Hiddify-Linux-x64.AppImage)
- [Github下载](https://github.com/hiddify/hiddify-next/releases) 

首先，下载软件Hiddify-Linux-x64.AppImage。从压缩模式中提取下载的文件，然后使用以下命令检查它是否有权执行。

假设下载的文件位于主文件夹中的下载中，因此运行以下命令。

ls -la ~/Downloads/hiddify-linux-x64.AppImage

如果输出如下：

rwxr-xr-x 1 user user 26272960 Sep 30 07:55 ~/Downloads/hiddify-linux-x64.AppImage

这意味着它具有 x 或可执行权限，可以运行它。否则，需要在终端中运行命令来添加执行权限。

第一次运行它时可以单击Language更改语言为中文，点击开始会进入配置界面。

点击“+新的配置文件”，打开以下免费账号的网址，找到ss或者v2ray节点的一键导入链接，复制链接，点击“剪贴板添加”。

[免费SS/SSR账号获取地址](https://gitlab.com/zhifan999/fq/-/wikis/ss%E5%85%8D%E8%B4%B9%E8%B4%A6%E5%8F%B7)

[免费v2ray账号获取地址](https://gitlab.com/zhifan999/fq/-/wikis/v2ray%E5%85%8D%E8%B4%B9%E8%B4%A6%E5%8F%B7)

***

**四、iOS免费翻墙软件**

iOS：[没有美区AppleID的翻墙教程](https://gitlab.com/zhifan999/fq/-/wikis/%E8%8B%B9%E6%9E%9C%E6%89%8B%E6%9C%BA%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6) [iOS注册美区Apple ID教程](https://gitlab.com/zhifan999/fq/-/wikis/iOS%E6%B3%A8%E5%86%8C%E7%BE%8E%E5%8C%BAApple-ID%E6%95%99%E7%A8%8B) 

***

**五、安卓免费翻墙软件**

安卓v2rayNG 客户端：[Github最新版下载](https://github.com/2dust/v2rayNG/releases) [Github镜像下载](https://jgithub.xyz/2dust/v2rayNG/releases)

点击软件主界面右上角的 ➕ 号按钮即可出现添加配置文件选项，如下图 V2rayNG 主界面所示，可以从剪贴板导入或扫描二维码或手动输入节点信息。复制节点一键导入链接后，选择从剪贴板导入。

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayng202502.png)

点击软件主界面右小角的 V 字图标启动代理，首次配置会提示是否创建代理，即软件界面中的网络链接请求，点击确定启动，如下图所示。

![](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/v2rayng202503.png)

启动成功后，主界面右下角的软件图标会变色代表启动成功。

***

有问题可以发邮件至海外邮箱rebeccalane27@gmail.com