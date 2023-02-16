一个基于ll.net的BDS插件
# 快速上手
LLMIRAI.NET
一个基于ll.net的BDS插件

## 前置准备

以及，你还需要：

- 一台联网的计算机
- 一个正常工作的人类大脑
- 一双勤劳的手

## 安装mirai环境

你也可以先了解：[什么是mirai](https://github.com/mamoe/mirai)。

虽然mirai的官方文档已经有了详细的配置教程，但是为了不让大家多看些文档，我们这里简单地介绍一下安装mirai的方法，如果你已经部署完成Mirai.NET所需要的mirai环境(**以及最新的`mirai-api-http`**)，这部分可以跳过。

注意，从这里开始，文档里所有的`mirai`都是指`mirai-console`。

### 安装 MCL

`MCL`(Mirai Console Loader Installer)是一个`mirai-console`的 CUI 封装，安装它就完事了。

首先访问`MCL`的[github release](https://github.com/iTXTech/mcl-installer/releases)，根据你的系统选择对应的安装器，通常来说你应该下载`mcl-installer-xx-windows-amd64.exe`，因为如果你用别的系统你应该不会继续看这个宝宝巴士文档。

![](https://i.loli.net/2021/08/04/tpKVqcEsbQHkRGJ.png)

那么，现在你已经下载好了`mcl-installer`，现在你需要把它放到一个文件夹里，然后运行它。通常来说，你应该只需要一直按`enter`键。

当`Press Enter to exit`出现，你就可以关闭安装器的窗口。

### 启动 MCL

下面就是安装好`MCL`的结果，你应该运行`mcl.cmd`这个命令脚本。

![](https://i.loli.net/2021/08/04/oeDvuIQGWMY4kOz.png)

运行之后，等到`main: mirai-console started successfully.`这行绿色字出现的时候，请先输入`/stop`来关闭`mcl.cmd`的运行窗口。因为我们还需要手动安装`mirai-api-http`插件。

### 安装和配置 mirai-api-http

首先访问[mirai-api-http release](https://github.com/project-mirai/mirai-api-http/releases) 页面，下载`jar`构件，下载完成后，把它放到`/plugins`目录下，然后再启动`mcl.cmd`。

![](https://i.loli.net/2021/08/04/dC35wLPz7rkcuj4.png)

同样的，等到`main: mirai-console started successfully.`这行绿色字出现的时候，先输入`/stop`来关闭`mcl.cmd`的运行窗口。再打开`/config/net.mamoe.mirai-api-http/setting.yml`文件。

用下面的内容覆盖原有的内容(来自[官方文档](https://docs.mirai.mamoe.net/mirai-api-http/#setting-yml-模板)):

```yaml
## 配置文件中的值，全为默认值

## 启用的 adapter, 内置有 http, ws, reverse-ws, webhook
adapters:
  - http
  - ws

## 是否开启认证流程, 若为 true 则建立连接时需要验证 verifyKey
## 建议公网连接时开启
enableVerify: true
verifyKey: 1234567890

## 开启一些调式信息
debug: false

## 是否开启单 session 模式, 若为 true，则自动创建 session 绑定 console 中登录的 bot
## 开启后，接口中任何 sessionKey 不需要传递参数
## 若 console 中有多个 bot 登录，则行为未定义
## 确保 console 中只有一个 bot 登陆时启用
singleMode: false

## 历史消息的缓存大小
## 同时，也是 http adapter 的消息队列容量
cacheSize: 4096

## adapter 的单独配置，键名与 adapters 项配置相同
adapterSettings:
  ## 详情看 http adapter 使用说明 配置
  http:
    host: localhost
    port: 8080
    cors: [*]

  ## 详情看 websocket adapter 使用说明 配置
  ws:
    host: localhost
    port: 8080
    reservedSyncId: -1
```

通常来说，你还需要自己修改`verifyKey`的值。

### 登录机器人账号

启动`mcl.cmd`，这次不用再关。

输入命令:`/login <qq> <密码>`，就可以登陆机器人账号了。通常来说，正常的机器人账号是可以直接登陆的，如果出现红色的错误提示，那么你可以根据`mcl.cmd`输出的提示文本找人帮忙或者自己解决。

到这里，Mirai.NET所需要的`mirai`环境已经配置好了。

#### 登录需要验证码

如果你登陆mcl弹出了下面的弹窗，请访问[TxCaptchaHelper](https://github.com/mzdluo123/TxCaptchaHelper)并按照提示操作。

![picture 1](https://s2.loli.net/2022/02/27/AztkmgU4o6W8nyT.png)  

## 安装LLMIRAI.NET


下载压缩包后解压到plugins目录下开服即可会自动s配置

以下是功能
![2.png](https://s2.loli.net/2023/02/14/AvmOY59ouxUGDRb.jpg)

写在后面：想要的功能可以评，论望5星好评
