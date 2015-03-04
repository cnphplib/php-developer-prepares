# 科学上网 (Cross the GFW)

把科学上网放在最前面，是因为个人认为 **好奇心 & 动手能力** 是许多优秀开发人员共有的特质；更为重要的是，在墙高度不定期加码的情况下，时刻掌握最新科学上网方法能一定程度上反应使用者对于网络协议的基本理解、服务器的操作管理能力、动手能力以及自我学习能力；同样的，各主流社区交流都以英文为主，计算机领域的大牛、信息多富集于中华大局域网之外，要想掌握最新的领域知识、获得第一手行业资料，熟练使用 **Google 而非百度、使用英文而非中文** 是技术人员的良好素质。

目前出墙的方式主要有，

## VPN 全局模式
 * PPTP 协议
 * L2TP/IPsec 协议
 * OpenVPN

  对比代理模式，VPN 模式是最容易/优先被墙识别并屏蔽的，因此出于稳定性和可维护性的考虑，个人推荐使用专业 VPN 服务商，而非自建 VPN：
    * [云梯](https://www.ytbit.com/) - 稳定、服务好
    * [曲径](https://getqujing.com/) - 价格稍贵，但物有所值

## 代理模式
 * [Goagent](https://github.com/goagent/goagent)
    GoAgent是利用Google App Engine的服务器资源，使用 Python 开发的代理软件。
 * [Shadowsocks](http://shadowsocks.org/)
    由于Shadowsocks使用socks5协议和可自定义密码的工业级算法加密，使得流量在网络传输过程中不易被他人读取。但是使用不可靠来源的Shadowsocks服务器可能会导致使用者的信息泄露。
 * SSH tunnel
    当用 SSH 连接到跳板机之后，SSH 可以在本地开启一个端口，本地的应用程序连接到本地的这个端口。相当于在本地建立了一个 Socks 代理服务器为本地的应用程序提供 Socks 代理。而这个 Socks 代理通过跳板机连接外网，Socks 代理和跳板机直接的数据通信是在 SSH 隧道里进行的，是安全的。

    更多信息请参考 IBM DeveloperWorks 技术文章 - [实战 SSH 端口转发](https://www.ibm.com/developerworks/cn/linux/l-cn-sshforward/)

## 相关工具：

  * SSH 客户端（Windows 环境，Linux、Mac 那都不是事儿）
    PuTTY, Bitvise, WinSCP, SecureCRT, Xshell...
    具体哪个就仁者见仁了，更多信息请参考 -  [Comparison of SSH Clients](http://en.wikipedia.org/wiki/omparison_of_SSH_clients)
  * [Polipo](http://www.pps.univ-paris-diderot.fr/~jch/software/polipo/) - Socks Proxy to HTTP Proxy
    因为上面几种方式得到的都是 Socks 协议的代理，Polipo 可以很方便的将 Socks 代理转为 HTTP 代理
  * [ProxyChains](https://github.com/rofl0r/proxychains-ng) - Run any program through HTTP or SOCKS proxy
    Proxychains 可以强制一个应用程序使用代理，它支持 HTTP、Socks、Socks5 这3种协议，而对整个系统没有影响。 
  * [SwitchyOmega](https://github.com/FelisCatus/SwitchyOmega) - Manage and switch between multiple proxies quickly & easily
    Google Chrome 浏览器的代理插件，轻松快捷地管理和切换多个代理设置。用于替代 SwitchySharp 插件的更新版本。
  * [FoxyProxy](http://getfoxyproxy.org/) - Advanced proxy management tool for Firefox
    FoxyProxy是Firefox下一款优秀的代理服务器管理扩展，它主要功能是管理Firefox代理服务器设置