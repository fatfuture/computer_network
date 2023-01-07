# 什么是DNS?

DNS 是计算机域名系统 (Domain Name System 或Domain Name Service) 的缩写，它是由解析器以及域名服务器组成的。

# 实作一

![](./image/snipaste20230101_182134.jpg)

# 实作二

![](./image/snipaste20230101_182444.jpg)

![](./image/snipaste20230101_182741.jpg)

# 实作三

![](./image/snipaste20230101_182835.jpg)

# 问题

上面秘籍中我们提到了使用插件或自己修改 hosts 文件来屏蔽广告，思考一下这种方式为何能过滤广告？如果某些广告拦截失效，那么是什么原因？你应该怎样进行分析从而能够成功屏蔽它？

hosts比DNS优先级高，用错误信息去屏蔽掉DNS上的信息。
具体情况请参考：https://www.cnblogs.com/hustskyking/p/hosts-modify.html


