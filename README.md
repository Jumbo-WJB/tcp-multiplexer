//http://mp.weixin.qq.com/s?__biz=MzAwNTYwMjM3Mw==&mid=2651680490&idx=1&sn=4850acabe57af8e79825e455d0466baa&chksm=80e3e3c0b7946ad61868d2f36b6b5f9b6226042a250d1f8dd537aa373e4462aa319e02033065&mpshare=1&scene=23&srcid=0223vVnzzrVYU1nrH94dyXO7#rd


# tcp-multiplexer
A TCP service multiplexer in Python

## 用途
&nbsp;&nbsp;&nbsp;&nbsp;在远程服务器只开放特定端口，但是需要支持不同应用访问的时候，如某服务器/防火墙只允许9000端口进行通信，但是此时我想要使用ssh服务，同时使用其http服务，或者其他服务。此时，可以使用该程序进行端口多路复用。

&nbsp;&nbsp;&nbsp;&nbsp;`tcp-multiplexer-demo.py`中的`PROTOCOL_RULES`可以根据需要进行配置，监听在本地的端口如：9000，接收到客户端的请求之后，会根据正则表达式去匹配相应的规则进行应用选择。

## 开发背景
想通过80端口，同时使用HTTP服务以及SSR服务

## 参考
- [https://github.com/darvid/emissary](https://github.com/darvid/emissary "A TCP service multiplexer")
- Python TCP Proxy
