**2025年11月26日更新。**

***

🚀 **Mac 启用第三方 APP 打开权限（允许“任何来源”）**

当 Mac 阻止第三方应用运行时，可以通过以下两种方式开启权限。

---

✅ **方法一：通过系统设置开启（如果已显示“任何来源”）**

1. 打开 **系统偏好设置 → 安全性与隐私 → 通用**  
2. 点击左下角 **🔒 锁图标**，输入密码解锁  
3. 将 **“允许从以下位置下载的应用”** 设置为 **“任何来源”**

---

💻 **方法二：终端启用“任何来源”（最通用、适用于多数情况）**

1. 打开 **终端（Terminal）**  
2. 输入以下指令并回车：
   sudo spctl --master-disable
3. 输入电脑密码（注意：输入时不会显示字符）
4. 回到 系统偏好设置 → 安全性与隐私 → 通用
5. 选择新增出现的 “任何来源” 选项

***

🚀 **Mac 解决“软件已损坏，无法打开”问题（强制运行）**

如果打开某些未签名软件时，提示：

- “xxx 已损坏，无法打开”
- “无法验证开发者”
- “已被隔离”

这是 macOS 自动给软件加上了隔离标记（Quarantine）。

可以使用以下方法强制运行。

- 方法：xattr -cr /Applications/你的App.app
- 示例：xattr -cr /Applications/v2rayN.app

***

**一、Mac v2rayN免费翻墙软件**

Mac客户端 v2rayN 7.15.7

**Apple M芯片-v2rayN-macos-arm64.dmg**

- [国外云盘下载](https://download.840899.xyz/v2rayN-macos-arm64.dmg)
- [Github下载](https://github.com/2dust/v2rayN/releases/download/7.15.7/v2rayN-macos-arm64.dmg)

**Intel芯片-v2rayN-macos-64.dmg**

- [国外云盘下载](https://download.840899.xyz/v2rayN-macos-64.dmg)
- [Github下载](https://github.com/2dust/v2rayN/releases/download/7.15.7/v2rayN-macos-64.dmg)

注意：由于安装包没有签名，会提示应用已损坏；安装后需要运行：xattr -cr /Applications/v2rayN.app 

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/v2rayn202508.png)

**安装教程如下**：

根据自己Mac的芯片类型，选择下载Mac v2rayN 客户端下载文件：
v2rayN-macos-arm64.dmg或 v2rayN-macos-64.dmg

双击打开下载文件后，v2rayN Installer 窗口弹出。将v2rayN图标拖到Applications图标：

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202501.jpg)

如果屏幕弹出窗口：

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202502.jpg)

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202503.jpg)

在设置中找到v2rayN 路径：设置Settings – General – About – System Report，点开 System Report: 

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202512.jpg)

在 System Report 的左边找到Software，点开其中 Applications，右边往下滑找到 v2rayN 客户端，点开，复制它的位置 Location: /Applications/v2rayN.app：

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202505.jpg)

到应用夹Applications box搜索TERMINAL，找到后点开，输入强制启动命令：
xattr -cr / Applications/v2rayN.app, 回车后输入本电脑密码（输入密码时屏幕不显示任何东西），回车：

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202506.jpg)

到应用夹Applications 里找到v2rayN图标，双击打开，参考此网站Mac 启用第三方 APP 打开权限（允许“任何来源”），在“设置” -“私隐和安全性” - “安全性”中，选择“仍要打开“，然后打开v2rayN客户端。

从节点网站一键复制相应节点，黏贴到v2rayN 左上角 “配置” Configurations 中的 Import Share Links from clipboard (Ctrl+V)。可黏贴导入多个节点:

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202507.jpg)

在v2rayN 屏幕下方代理 Proxy选项中选 “Set system proxy”，在其隔壁右边V3选项中选 “V3-全局 (Global)”:

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202508.jpg)

右击已导入节点选择 “Set as active Configuration (Enter)”（或直接回车），选择后被选节点显示红色 “Active”图示，屏幕右上角v2rayN 图标变红色，此时应已连上：

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202509.jpg)

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/macv2rayn202510.jpg)

此时外网应连接上。

[点我获取免费v2ray账号](https://gitlab.com/zhifan999/fq/-/wikis/v2ray%E5%85%8D%E8%B4%B9%E8%B4%A6%E5%8F%B7)

**二、Mac Hiddify免费翻墙软件**

Mac客户端 Hiddify 2.5.7 文件名称：Hiddify-MacOS.dmg

[下载地址1](https://download.979862.xyz/Hiddify-MacOS.dmg) [下载地址2](https://download.840899.xyz/Hiddify-MacOS.dmg) [下载地址3](https://download.186408.xyz/Hiddify-MacOS.dmg) [github最新版下载](https://github.com/hiddify/hiddify-app/releases)

MAC安装：

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac-002.jpg)

MAC启动：

⚠️【必读】如提示：无法打开“Hiddify”，看下图解决方案【按1、2、3、4 红字顺序操作】。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac-001.png)

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac-003.jpg)

安装好后，点击+新的配置文件，找到v2ray节点的一键导入链接，复制链接，点击“剪贴板添加”。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac-004.jpg)

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac-005.jpg)

[点我获取免费v2ray账号](https://gitlab.com/zhifan999/fq/-/wikis/v2ray%E5%85%8D%E8%B4%B9%E8%B4%A6%E5%8F%B7)


***

**三、Mac ss/ssr免费翻墙软件**

[全平台SS/SSR客户端下载汇总](http://www.mediafire.com/folder/sfqz8bmodqdx5/shadowsocks相关客户端)

[点我获取最新免费ss或ssr账号](https://gitlab.com/zhifan999/fq/-/wikis/ss%E5%85%8D%E8%B4%B9%E8%B4%A6%E5%8F%B7)

具体步骤：

**SSR客户端下载地址：** 

 ShadowsocksX-NG-R8.dmg

- [国外云盘下载](https://download.840899.xyz/ShadowsocksX-NG-R8.dmg)
- [Github最新版下载](https://github.com/shadowsocksr-backup/ShadowsocksX-NG/releases/download/1.4.2-R8-subscribe-alpha-3/ShadowsocksX-NG-R8.dmg) 


***

以SSR客户端ShadowsocksX-NG-R8.dmg为例：

打开下载的DMG文件，双击打开或者右键打开。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/ssr202501.png)

右上方出现程序图标，点击图标“服务器”–“打开服务器设定”。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/ssr202502.png)

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/ssr202503.png)

点击 + 进入服务器界面。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/ssr202504.png)

手动填写服务器信息，包括服务器ip、端口、加密方式、密码、协议和混淆，每一个参数都要填写正确，错1个都会用不了。然后点击OK。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/ssr202505.png)

代理模式选择全局代理Global Mode

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/ssr202508.png)

最后选择启用软件。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/ssr202509.png)


***


**四、高速机场(付费)**

[w1.v2free.cyou](https://w1.v2free.cyou/auth/register?code=UsUP)是海外人士运营的高速翻墙服务，2020年开始已稳定运行3年。支持Windows/MAC/iOS/安卓/Linux/路由器等各平台高速翻墙：解锁大多数流媒体（Netflix、TVB、HKTV、ViuTV等），1080P高清视频、4K高清视频秒开，超低延迟。任意套餐的高速节点都支持访问openAI ChatGPT。

节点位置有台湾、香港、韩国、日本、美国、新加坡等，付费套餐节点包括v2ray节点和SS节点。截至2023年9月14日，节点共100个左右。

试用套餐5元（5天）、月付套餐A 20元、月付套餐B 39元、月付套餐C 58元、年付套餐A 168元、年付套餐A2 218元等，[套餐购买](https://w1.v2free.cyou/auth/register?code=UsUP)

详细介绍及购买方法：https://gitlab.com/zhifan999/fq/-/wikis/V2free%E6%9C%BA%E5%9C%BA

有问题也可以问在线客服。

***

**五、Mac 神盾VPN(付费)**

免费试用，有限速。

Mac版：https://apps.apple.com/app/tipas-vpn/id6749783838

有两个网站可以购买服务：

官网：https://cn.tipas.net

镜像：https://tipasvpn.com

使用支付宝购买亚马逊礼品卡很方便，在结账和常见问题里面有说明和购买教程视频：

https://tipasvpn.com/faq

8折优惠码 TYZH 可以在两个网站上使用，大小写没有关系。

官网：https://cn.tipas.net/shop2/

镜像站：https://sd0501.com

有问题联系官方客服邮箱：support@tipas.net

图文教程:

第一步：如图点击“前往”，再点击"应用程序"。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac1.png)

第二步：如图双击dmg文件打开，将Tipas拖拽到“应用程序”窗口里面。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac2.png)

第三步：右键单击“应用程序”中的Tipas，选择“打开”，系统弹出“Tipas是从互联网下载的App。您確定要打开它吗？”。点击“打开”。

第四步：如图点击“打开安全性偏好设置"。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac3.png)

第五步：如图点击。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac4.png)

第六步：如图点击。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac5.png)

第七步：如图点击。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac6.png)

第八步：如图点击。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac7.png)

第九步：如图。

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/mac8.png)

第十步：

点击第九步图里的右上角圆标设置账号密码和刷新中继器。(需要购买服务后设置帐号密码，然后刷新中继器。)


***

### 🌍 翻墙后推荐网站：

🔍 **搜索类**：[Google](https://www.google.com)  
📰 **新闻类**：[动态网](http://dongtaiwang.com) | [大纪元](https://www.epochtimes.com/gb) | [阿波罗新闻网](https://www.aboluowang.com) | [禁书网](https://www.bannedbook.org/bbook.php)  
📺 **视频类**：[YouTube](https://www.youtube.com) | [干净世界](https://www.ganjing.com/zh-CN) | [新唐人电视台](https://www.ntdtv.com)  
🌐 **社交类**：[X(推特)](https://x.com/)  
📻 **广播电台类**：[希望之声](https://www.soundofhope.org)  
🎨 **文化艺术类**：[神韵](https://zh-cn.shenyun.org/what-is-shen-yun) | [神韵作品](https://www.shenyuncreations.com/zh-CN)  
📚 **百科类**：[维基百科](https://zh.wikipedia.org/wiki/Wikipedia:%E9%A6%96%E9%A1%B5)  
🤖 **AI 类**：[ChatGPT](https://chatgpt.com/) | [DuckDuckGo-AIChat](https://duckduckgo.com/?q=DuckDuckGo+AI+Chat&ia=chat&duckai=1) | [Grok](https://grok.com/) | [Gemini](https://gemini.google.com/app) | [Copilot](https://copilot.microsoft.com/)  | [DeepAI](https://deepai.org/)


**▶️ YouTube频道推荐**

[文昭谈古论今](https://www.youtube.com/@wenzhaoofficial/videos) | [时事金扫描](https://www.youtube.com/@時事金掃描/videos)  | [希望之声TV](https://www.youtube.com/@SOH_TV/streams)  | [天亮论政](https://www.youtube.com/@TianliangZhang/streams)   | [新闻最嘲点姜光宇](https://www.youtube.com/@MrFunnyNewsJGY/videos)     |   [Leonard](https://www.youtube.com/channel/UC1mx_wcSHtfpLk5N_zY0TRg/videos)   |   [人民报](https://www.youtube.com/@人民報renminbao/videos)  | [文昭思绪飞扬](https://www.youtube.com/channel/UCTu_hTaVf3DJMpMIyOAq2Ew/videos)  | [信不信由你](https://www.youtube.com/@xbxynfun/videos) | [晨曦晓屋](https://www.youtube.com/@chenxixiaowu/videos) 


**📺 视频推荐**

- [纪录片《江油事件》](https://www.youtube.com/watch?v=7qjZ89NSwYs)
- [1989六四事件:广场备忘录-BBC News 中文](https://www.youtube.com/watch?v=ExqqdUXXdgA&ab_channel=BBCNews%E4%B8%AD%E6%96%87)
- [第51届哥伦布国际电影电视节荣誉奖——《伪火》](http://cn.ntdtv.com/gb/2014/01/07/a24016.html) 
- [关于台湾的5大真相](https://www.youtube.com/watch?v=O2hbHbdYG2w&ab_channel=Leonard)
- [《九评》历史真相系列纪录片](https://www.ntdtv.com/gb/2023/02/04/a103641795.html)
- [北宋预言《梅花诗》](https://www.ganjingworld.com/zh-CN/video/1h1avcli4jj3fuuswOXnh1ULh1pc1c)
- [“三阿哥”的戏剧人生（上）](https://www.ntdtv.com/gb/2021/02/12/a103052600.html)
- [“三阿哥”的戏剧人生（中）](https://www.ntdtv.com/gb/2021/02/25/a103061565.html)
- [“三阿哥”的戏剧人生（下）](https://www.ntdtv.com/gb/2021/03/24/a103080241.html)

**📺 神韵视频推荐**

- [2026神韵晚会预告片](https://www.shenyuncreations.com/zh-CN/video/_video_67f730a0899c4920875572a35e7158f6/Shen-Yun-2026-Official-Trailer)
- [神韵晚会观众反馈(2025)](https://www.shenyuncreations.com/zh-CN/video/_video_84840ca70db041bea52603b4bb464b2e/Shen-Yun-Audience-Reviews-2025)
- [关于神韵的五个事实](https://www.shenyuncreations.com/zh-CN/video/_video_6383b459b549440897914760fe302331/5-Things-About-Shen-Yun-You-Probably-Didnt-Know?pid=up-next)
- [如何炼就神韵制作部](https://www.shenyuncreations.com/zh-CN/video/_video_a81c6d107bc242299e1779afb3f2ae9e/What-Does-It-Take-to-be-a-Shen-Yun-Production-Member?pid=p_QN0mwWlwQQWV&view=)
- [神韵领舞演员专访-王琛](https://www.shenyuncreations.com/zh-CN/video/_video_83840b81df8a4aaeae36addd762cd715/Meet-Principal-Dancer-Angelia-Wang?pid=p_Q3bw9EA4TyKu&view=)
- [神韵艺术团简介](https://www.shenyuncreations.com/zh-CN/video/_video_98e3a94cfcda495e9364572c3481f938/Shen-Yun-Performing-Arts-Intro?pid=up-next)
- [神韵艺术家的摇篮—飞天大学剪影](https://www.shenyuncreations.com/zh-CN/video/_video_d02cce6f428843d3bafa1acf596d6f22/Student-Life-at-Fei-Tian-College?pid=p_EVJnxzchTYmh&view=)


***

有问题可以发邮件至海外邮箱rebeccalane27@gmail.com