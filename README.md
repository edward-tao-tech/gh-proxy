# gh-proxy

## 简介

github release、archive以及项目文件的加速项目，支持clone，有Cloudflare Workers无服务器版本以及Python版本


## python版本和cf worker版本差异

- python版本支持进行文件大小限制，超过设定返回原地址 [issue #8](https://github.com/hunshcn/gh-proxy/issues/8)

- python版本支持特定user/repo 封禁/白名单 以及passby [issue #41](https://github.com/hunshcn/gh-proxy/issues/41)

## 使用


***大量使用请自行部署，以上域名仅为演示使用。***

访问私有仓库可以通过

`git clone https://user:TOKEN@ghproxy.com/https://github.com/xxxx/xxxx` [#71](https://github.com/hunshcn/gh-proxy/issues/71)

以下都是合法输入（仅示例，文件不存在）：

- 分支源码：https://github.com/hunshcn/project/archive/master.zip

- release源码：https://github.com/hunshcn/project/archive/v0.1.0.tar.gz

- release文件：https://github.com/hunshcn/project/releases/download/v0.1.0/example.zip

- 分支文件：https://github.com/hunshcn/project/blob/master/filename

- commit文件：https://github.com/hunshcn/project/blob/1111111111111111111111111111/filename

- gist：https://gist.githubusercontent.com/cielpy/351557e6e465c12986419ac5a4dd2568/raw/cmd.py

