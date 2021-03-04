'SOAP'

## SOAP简介
SOAP 是基于 XML 的简易协议，可使应用程序在 HTTP 之上进行信息交换。

或者更简单地说：SOAP 是用于访问网络服务的协议。

SOAP 指简易对象访问协议

SOAP 是一种通信协议

SOAP 用于应用程序之间的通信

SOAP 是一种用于发送消息的格式

SOAP 被设计用来通过因特网进行通信

SOAP 独立于平台

SOAP 独立于语言

SOAP 基于 XML

SOAP 很简单并可扩展

SOAP 允许您绕过防火墙

SOAP 将被作为 W3C 标准来发展


## 语法规则

这里是一些重要的语法规则：

SOAP 消息必须用 XML 来编码

SOAP 消息必须使用 SOAP Envelope 命名空间

SOAP 消息必须使用 SOAP Encoding 命名空间

SOAP 消息不能包含 DTD 引用

SOAP 消息不能包含 XML 处理指令

SOAP 消息的基本结构

```
<?xml version="1.0"?>
<soap:Envelope
xmlns:soap="http://www.w3.org/2001/12/soap-envelope"
soap:encodingStyle="http://www.w3.org/2001/12/soap-encoding">

<soap:Header>
...
</soap:Header>

<soap:Body>
...
  <soap:Fault>
  ...
  </soap:Fault>
</soap:Body>

</soap:Envelope>
```