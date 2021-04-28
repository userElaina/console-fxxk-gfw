# wsl cmd fuck gfw
\#新手向
\#个人笔记

关于如何在WSL和cmd里使用代理这件事

经测试,只有cmd可以,powershell不行.

(powershell怎么弄如果有知道的欢迎留言)

本文假设设置代理端口为1001.

端口是多少在这里看(Windows 10):

![image](https://user-images.githubusercontent.com/80948381/116335193-03642980-a809-11eb-9890-6253d6a88fd0.png)

其它系统请自行Google.

---
v2rayNG
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
注意：关于 v2rayN
---
v2rayN里设置端口为1000(如下图)时,实际端口会是1001(即+1了).

![QQ图片20210428095802](https://user-images.githubusercontent.com/80948381/116334722-4376dc80-a808-11eb-8b6f-0db5a7a55daa.png)

我也不知道为什么要+1.
