# TinyWebServer

[参考前辈博客](https://blog.csdn.net/weixin_51322383/article/details/130464403)

以下内容摘自 **什么是 WebServer**

WebServer 是一个 B/S 架构，即浏览器扮演客户端，而 WebServer 就是服务器程序，或者说是运行这个服务器软件的计算机。

其主要的功能就是通过 HTTP 协议与客户端（Browser）进行通信，来接收、存储、处理来自客户端的 HTTP 请求，并对其请求做出 HTTP 响应，这个响应是指发送响应报文（文件、网页等）或者是一个 Error 信息。

一个 WebServer 如何和用户进行通信，就需要在浏览器输入域名或者 IP 地址:端口号，浏览器会先将你的域名解析成响应的 IP 地址（通过 DNS）或者直接根据你的 IP:Port 向对应的 Web 服务器发送一个 HTTP 请求。这个过程需要 TCP 协议的三次握手建立和目标 Web 服务器的连接，然后 HTTP 协议生成针对该 Web 服务器的 HTTP 请求报文，这个报文里面包括了请求行、请求头部、空行和请求数据四个部分（后面再细讲），通过 TCP/IP 协议发送到 Web 服务器上。
