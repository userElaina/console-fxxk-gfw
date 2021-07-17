# How to use proxies in some console
\#新手向
\#个人笔记

本文假设设置 `HTTP` 代理端口为 `1001`.

---
### WSL
```sh
export http_proxy="http://127.0.0.1:1001"
export https_proxy="http://127.0.0.1:1001"
```
---
### cmd
```sh
set http_proxy=http://127.0.0.1:1001
set https_proxy=http://127.0.0.1:1001
```
---
### PowerShell
```sh
$Env:http_proxy="http://127.0.0.1:1001"
$Env:https_proxy="http://127.0.0.1:1001"
```
---
### Git
```sh
git config --global https.proxy http://127.0.0.1:1080
git config --global https.proxy https://127.0.0.1:1080
git config --global --unset http.proxy
git config --global --unset https.proxy
npm config delete proxy
```
---
## 如何查看端口

### Windows 10 全局模式:

![image](https://user-images.githubusercontent.com/80948381/116337014-14fb0080-a80c-11eb-8c2c-1af295cb690c.png)

### v2rayN

![image](https://user-images.githubusercontent.com/80948381/126021355-a12f0d58-bcf7-4815-830e-6a9ef0c5b873.png)

#### 关于 v2rayN 开启全局模式时

v2rayN 里设置端口为 `1000` (如下图)并开启全局模式时,实际系统代理端口会是 `1001` (即+1了).

这是因为设置 `Socks5` 端口为 `1000` 的同时自动设置 `HTTP` 端口为 `1001`.

![image](https://user-images.githubusercontent.com/80948381/116334722-4376dc80-a808-11eb-8b6f-0db5a7a55daa.png)

### Clash

![image](https://user-images.githubusercontent.com/80948381/126021364-d801cb12-af14-4009-8a30-0141bca34869.png)

### 其它系统/软件请自强

