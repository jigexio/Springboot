# HTTP请求和响应过程

## 1.在浏览器里输入网址,域名（IP地址）解析

![](C:\Users\LENOVO\Desktop\img\QQ图片20190531213215.png)

浏览器根据访问的域名找到其IP地址,过程如下：

- 浏览器缓存：首先, 浏览器会缓存DNS记录一段时间。在浏览器的DNS缓存中查找域名对应的IP地址。

- 系统缓存：如果在浏览器缓存里没有找到需要的域名，浏览器会做一个系统调用，就会在操作系统的DNS缓存中进行查找。

- 路由器缓存：如果系统缓存也没找到需要的域名，则会向路由器发送查询请求，在路由器的DNS中查找。
- ISP缓存：如果依然没找到需要的域名，则最后要查的就是ISP缓存DNS的服务器。在这里一般都能找到相应的缓存记录

![](C:\Users\LENOVO\Desktop\img\1352475214_6561.png)





## 2.浏览器与web服务器建立一个 TCP 连接

## 3.Web浏览器想Web服务器发送请求命令

http请求的常见请求方法有GET、POST、HEAD

#### GET、POST的区别

![](C:\Users\LENOVO\Desktop\img\20180910171105577.png)

## 4.服务器永久重定向响应

应答第一部分就为版本号和协议状态码：HTTP/....   200  OK

## 5.浏览器跟踪重定向的地址，并向改地址发送http请求

## 6.服务器处理请求

## 7.服务器发回一个HTML响应

## 8.释放TCP连接

若connection 模式为close，则服务器主动关闭TCP 连接，客户端被动关闭连接，释放TCP 连接;若connection 模式为keepalive，则该连接会保持一段时间，在该时间内可以继续接收请求

## 9. 客户端浏览器解析HTML内容

客户端将服务器响应的 html 文本解析并显示

## 10. 浏览器获取嵌入在HTML中的对象

