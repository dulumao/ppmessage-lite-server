[In English](/README.md)

# PPMessage Lite Server - 皮皮消息，即插即用，纯Python实现。

PPMessage Lite Server 是配合 [PPMessage 在线服务](https://ppmessage.cn) 提供的一个精简的消息服务器，PPMessage Lite Server 能够在接口级别与 [PPMessage 在线服务](https://ppmessage.cn)兼容，其目标为 [PPMessage 在线服务](https://ppmessage.cn)的开发者提供一个可以本地部署的用来测试服务器，方便开发调试。

PPMessage Lite Server 建议部署到 macOS 上，其次 Debian Linux，再其次选择 Windows。


## 快速上手

### 下载代码

```bash
git clone https://github.com/PPMESSAGE/ppmessage-lite-server
cd ppmessage
```

### 安装依赖

> Debian/Ubuntu

```bash
bash ppmessage/scripts/set-up-ppmessage-on-linux.sh
```

> macOS


```bash
bash ppmessage/scripts/set-up-mac-on-linux.sh
```

> Windows

Windows需要的额外操作请参考[文档](install-ppmessage-on-windows.md)

### 执行


```bash
./config.py --email=你的邮箱地址 --password=初始化密码
```

```bash
./lite.py
```

> 删除文件 ppmessage/bootstrap/config.json，再运行 main.py 就可以重新配置。
> 如果你通过 github 更新了代码，那么需要重新运行 config.py。<strong>这点非常重要！</strong>

打开浏览器访问 http://127.0.0.1:8945，用你配置的`邮箱地址`和`初始化密码`登录。

> 就是这些，不工作？请将日志贴到 Github issue 中，谢谢！

## 版权 

> 使用前请仔细阅读版权声明。

本项目的源代码是按照 Apache License Version 2 开源的，其版权归属于原作者，并且只允许在单网站或者单应用和单客服上使用 PPMessage 及其衍生项目，如果想利用 PPMessage 的全部或者部分代码提供多租户（多站点）服务，请联系作者获取商业许可。

[Apache License Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)

Copyright (c) 2010-2017, PPMESSAGE team and contributors - https://www.ppmessage.com and https://github.com/PPMESSAGE/ppmessage

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.



## 其他项目

* [PPMessage Lite Server](https://github.com/PPMESSAGE/ppmessage-lite-server)

* [PPCom iOS SDK](https://github.com/PPMESSAGE/ppcom-ios-sdk)

* [PPCom Android SDK](https://github.com/PPMESSAGE/ppcom-android-sdk)
