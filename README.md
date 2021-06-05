# How to use proxies in WSL & cmd
\#新手向
\#个人笔记

关于如何在WSL和cmd里使用代理这件事

经测试,只有cmd可以,powershell不行.

(powershell怎么弄如果有知道的欢迎留言)

本文假设设置代理端口为 `1001`.

端口是多少在这里看(Windows 10):

![image](https://user-images.githubusercontent.com/80948381/116337014-14fb0080-a80c-11eb-8c2c-1af295cb690c.png)

其它系统请自行Google.

---
WSL
---
```sh
export http_proxy="http://127.0.0.1:1001"
export https_proxy="http://127.0.0.1:1001"
```
---
CMD
---
```sh
set http_proxy=http://127.0.0.1:1001
set https_proxy=http://127.0.0.1:1001
```
---
注意：关于 v2rayN 开启全局模式时
---
v2rayN里设置端口为 `1000` (如下图)并开启全局模式时,实际系统代理端口会是 `1001` (即+1了).不是全局模式不用+1.

![image](https://user-images.githubusercontent.com/80948381/116334722-4376dc80-a808-11eb-8b6f-0db5a7a55daa.png)

我也不知道为什么要+1.
