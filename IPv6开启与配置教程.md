# IPv6开启与配置教程

**2025年10月26日更新。**

适用于 **Windows 7/8/10/11、Linux、macOS，以及路由器 (TP-LINK 示例)**。  
同时补充了手机端的 IPv6 开启说明。

⚠️通知：2025年8月20日凌晨 00:34–01:48（UTC+8），大陆网络发生突发性大规模异常，境外ipv4 443 端口（HTTPS 加密访问）流量在此期间一度被全面屏蔽。虽然持续时间仅一小时左右，但不少人推测这可能是长城防火墙（GFW）升级后的深夜测试演练。根据网络社区反馈，当时极端情况下 IPv6 网络翻墙并未受阻。考虑到未来类似大规模封锁或将成为常态，因此有必要提前做好准备：学习如何开启并使用 IPv6 网络。

---

**✅ 常见中国大陆 IPv6 前缀**：

- `2408:xxxx:...`  — 中国电信 / 联通 / 移动常见
- `2409:xxxx:...`  — 中国联通 / 移动常见
- `240e:xxxx:...`  — 中国电信常见
- `240c:xxxx:...`  — 常见于中国电信
- `2402:xxxx:...`  — 较少见，也属于大陆 IPv6 网段
- `2001:da8:xxxx:...` — 教育网 CERNET（高校/科研网络）

说明：以上均为来自 APNIC 分配给中国大陆运营商的 IPv6 地址前缀。

**❌ 如果只有这种本地链接 IPv6 地址**：

- `fe80::xxxx:...` — 这不算公网

那说明你 IPv6 没真的启用，只是系统启用了本地回环功能。

---

## 一、路由器（TP-LINK 示例）

### 1. 路由器IPv4上网方式为“宽带拨号上网”，IPv6选“宽带拨号上网”
- 若路由器的上网方式为IPv4宽带拨号，且拨号成功后能正常上网，路由器的上网设置界面，如下图： 

![tplink图1](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/tplink-1.png)

- 在“路由器管理界面→路由设置→IPv6设置”中，将IPv6功能开启，WAN口连接类型选择宽带拨号上网，并勾选“复用IPv4拨号链路”，然后点击“连接”，如下图：

![tplink图2](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/tplink-2.png)

### 2. 路由器IPv4上网方式为“自动获得IP地址”，IPv6选“桥模式”
- 若路由器的上网方式为自动获得IP地址，且获取IP地址后能正常上网，路由器的上网设置界面，如下图：

![tplink图3](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/tplink-3.png)

- 则在“路由器管理界面→路由设置→IPv6设置”中，将IPv6功能开启，WAN口连接类型选择“桥模式”，点击“保存”，如下图：

![tplink图4](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/tplink-4.png)

资料来源：https://smb.tp-link.com.cn/service/detail_article_4739.html

⚠️ 注意：一般路由器设备的底部有登录路由器方法，包括路由器网址、用户名和密码。各个路由器开启 IPv6 方法可能有差异，如果不成功，建议联系路由器官方客服或者网上搜索自己牌子的路由器ipv6开启方法。

---

## 二、Windows 7/8/10/11 IPv6 配置

![Windows开启ipv6图1](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/2025-ipv6-1.png)

![Windows开启ipv6图2](https://cdn.jsdelivr.net/gh/Alvin9999-newpac/pac2/softimag/2025-ipv6-2.png)

1. 打开 **控制面板 → 网络和共享中心 → 更改适配器设置**  
2. 右键当前网络连接 → **属性**  
3. 勾选 **Internet 协议版本 6 (TCP/IPv6)** → **确认**  
4. IPv6 地址和 DNS 服务器推荐设置为 **自动获取**  

---

## 三、macOS IPv6 配置

1. 打开 **系统偏好设置 → 网络**  
2. 选择当前网络（Wi-Fi 或以太网） → **高级 → TCP/IP**  
3. 配置 IPv6 模式：  
   - **自动**（默认，从 ISP/路由器获取）  
   - **手动**（输入 IPv6 地址/64 + 网关 + DNS）  

---

## 四、Linux IPv6 配置

### 1. 查看 IPv6 状态
- ip -6 addr show

### 2. 临时配置 IPv6
- sudo ip -6 addr add 2001:db8::1234/64 dev eth0  
- sudo ip -6 route add default via 2001:db8::1 dev eth0  

### 3. 永久配置

#### Ubuntu (Netplan)
- 编辑 `/etc/netplan/01-netcfg.yaml`：  
  - network:  
    - version: 2  
    - ethernets:  
      - eth0:  
        - dhcp4: no  
        - dhcp6: yes  
        - addresses: 2001:db8::1234/64  
        - gateway6: 2001:db8::1  
        - nameservers:  
          - addresses: [2001:4860:4860::8888, 2606:4700:4700::1111]  

- 应用配置：  
  - sudo netplan apply  

#### CentOS / RHEL
- 编辑 `/etc/sysconfig/network-scripts/ifcfg-eth0`：  
  - IPV6INIT=yes  
  - IPV6ADDR=2001:db8::1234/64  
  - IPV6_DEFAULTGW=2001:db8::1  
  - DNS1=2001:4860:4860::8888  
  - DNS2=2606:4700:4700::1111  

- 重启网络：  
  - sudo systemctl restart network


## 五、手机 IPv6 开启与配置

- 手机网络（电话卡）默认由运营商自动分配 IPv6 地址。  
- 开启手机热点后，连接的电脑也会自动获取 IPv6 网络。  

---

## 六、检测 IPv6

### 1. 浏览器检测
- 打开 [https://testipv6.cn](https://testipv6.cn)  
- 若能显示 IPv6 地址并通过测试，说明 IPv6 已启用  

### 2. 命令行检测

#### Windows
- 打开命令提示符（CMD）  
- 输入：ipconfig  
- 在网络适配器下可看到 **IPv6 地址**

**常见中国大陆 IPv6 前缀**：

- `2408:xxxx:...`  — 中国电信 / 联通 / 移动常见
- `2409:xxxx:...`  — 中国联通 / 移动常见
- `240e:xxxx:...`  — 中国电信常见
- `240c:xxxx:...`  — 常见于中国电信
- `2402:xxxx:...`  — 较少见，也属于大陆 IPv6 网段
- `2001:da8:xxxx:...` — 教育网 CERNET（高校/科研网络）

说明：以上均为来自 APNIC 分配给中国大陆运营商的 IPv6 地址前缀。

#### macOS / Linux
- 打开终端  
- 输入：ip -6 addr show  
- 若能看到以 `2001:`、`2408:`、`2409:` 等开头的 IPv6 地址，即为启用成功  

### 3. Ping 测试
- Windows：ping -6 www.baidu.com
- Linux / macOS：ping6 www.baidu.com  
- 若能正常返回数据包，说明 IPv6 网络可用  

***

教程如果有需要完善的地方，可以发邮件至海外邮箱rebeccalane27@gmail.com