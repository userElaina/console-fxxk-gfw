# wsl cmd fuck gfw
关于如何在WSL和cmd里使用代理这件事

\# 新手向

---
v2rayNG
---
(假设v2ray设置端口为1000)

端口是多少在这里看：

![QQ图片20210428095802](https://user-images.githubusercontent.com/80948381/116334722-4376dc80-a808-11eb-8b6f-0db5a7a55daa.png)

WSL
```sh
export http_proxy="http://127.0.0.1:1001"
export https_proxy="http://127.0.0.1:1001"
```

cmd
```sh
set http_proxy=http://127.0.0.1:1001
set https_proxy=http://127.0.0.1:1001
```
我也不知道为什么要+1.

---
其它
---
(假设设置端口为1000)

WSL
```sh
export http_proxy="http://127.0.0.1:1000"
export https_proxy="http://127.0.0.1:1000"
```

cmd
```sh
set http_proxy=http://127.0.0.1:1000
set https_proxy=http://127.0.0.1:1000
```
