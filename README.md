# FakeWechatVersion

虚拟 Windows 微信版本，解决微信弹窗 "当前客户端版本过低,请前往应用商店升级到最新版本客户端后再登录"。

目前已兼容 `3.9 -> 4.x` 的版本伪装与启动场景。

## 用法：

### 1. 源码运行:
```shell
git clone https://github.com/ThinkerWen/FakeWechatVersion.git
cd FakeWechatVersion
python -m pip install pymem
# c为当前微信版本，t为目标微信版本
python fake_wechat_version.py c=3.9.6.33 t=3.9.12.51
```

### 2. 编译版运行
在 [Release](https://github.com/ThinkerWen/FakeWechatVersion/releases) 页面下载最新版 `fake_wechat.exe`。

请将 `fake_wechat.exe` 放在微信安装目录下，与 `WeChat.exe` 或 `Weixin.exe` 放在同一目录中。

双击 `fake_wechat.exe` 即可直接启动微信；

如果需要指定版本伪装，也可以执行：
```shell
fake_wechat.exe c=3.9.6.33 t=3.9.12.51
```
