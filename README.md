# wsl powershell fuck gfw
关于如何在WSL和cmd里使用代理这件事

---
v2rayNG
---
(假设v2ray设置端口为1000)

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
clash
---
(假设clash设置端口为1000)

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
