通过修改流程文件，使用Lienol's openwrt dev-19.07（平稳版）在线编译passwall服务、在线编译smartdns服务

修改流程文件REPO_URL: 不同库地址（默认Lienol的https://github.com/Lienol/openwrt 或者lean的https://github.com/coolsnowwolf/lede.git）；REPO_BRANCH: 不同分支 （以Lienol OpenWrt源码为例分支dev-master 激进；dev-19.07 OpenWrt官方平稳版；dev-lean-lede lean的源码）。

通过修改diy.sh文件可以自定义默认IP，登陆密码,增加smartdns源

修改流程文件触发条件。

在触发工作流程后，在 Actions 页面等待执行到SSH connection to Actions步骤，会出现下面信息：

To connect to this session copy-n-paste the following into a terminal or browser:

ssh Y26QeagDtsPXp2mT6me5cnMRd@nyc1.tmate.io

https://tmate.io/t/Y26QeagDtsPXp2mT6me5cnMRd

复制 SSH 连接命令粘贴到终端内执行，或者复制链接在浏览器中打开使用网页终端，登陆云menuconfig。

命令：cd openwrt && make menuconfig

新手参考OpenWrt MenuConfig设置和LuCI插件选项说明

完成后按快捷键Ctrl+D或执行exit命令退出，后续编译工作将自动进行。

地址：192.168.123.1

账户：root

密码：password


## 插件

* passwall

* ssrp+

* adbyby plus

* aria2

* smartdns

* ddns

等...
