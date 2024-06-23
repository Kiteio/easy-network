# 广东财经大学校园网双击登录

## 快速开始
1. 将 [校园网登录.cmd](校园网登录.cmd) 保存到本地（克隆或直接复制内容）
2. 使用**记事本**（右键文件，点击**在记事本中编辑**）或其他编辑工具打开 [校园网登录.cmd](校园网登录.cmd)，配置以下内容。如果不知道 ip 请参考[如何获取 ip](#如何获取-ip)
    ```commandline
    set name=学号
    set pwd=校园网密码
    set ip=ip
    ```
   示例：
   ```commandline
   set name=12345678910
   set pwd=abcdefg
   set ip=192.168.1.1
   ```
3. 双击运行脚本（记得先连上校园网）

## 如何获取 ip
> 网线和 wifi 的 ip 是不同的，我使用的是网线的 ip，然后连 wifi 也能登录验证，挺奇怪。
### 方法一
1. 连接校园网， 打开[链接](http://100.64.13.17/drcom/chkstatus?callback=dr1002&jsVersion=4.1.3&v=4833&lang=zh)
2. `Ctrl`+`F`查找 **v4ip**

### 方法二（Windows）
`设置` > `网络和 Internet` > `属性` > `IPv4 地址`
### 方法三（Windows）
1. 打开 cmd（`Win`+`R`，输入 **cmd** 回车）
2. 输入以下命令
    ```commandline
    ipconfig
    ```
3. 根据连接方式查找
- 网线：`以太网适配器 以太网 2` > `IPv4 地址`
- wifi：`无线局域网适配器 WLAN` > `IPv4 地址`
