---
author: 韩建伟
title:  "RESTful API"
date:   2022-03-18
---

# RESTful架构

REST = Representational State Transfer

- [Roy Thomas Fielding][rest_paper]提出
- [RESTful架构的解释][ruan]

# 交互过程

![rest_cs][]

# 设计规范

- [RESTful API 设计指南][rest_guide]
- [RESTful API 设计最佳实践][rest_best_practice]([中文][rest_best_practice_cn])
- 参考现有系统的API设计（如[GitHub API][]）

![rest_img][]

# 数据格式

- [JSON][]
- [XML][]
- [JSON vs XML][]

# 测试

- [ApiFox](https://www.apifox.cn)
- [Postman][]
- [httpie][]

# 资源

- [Awesome REST][]

# RPC

- Remote Procedure Call，远程过程调用
- 远程请求服务，无需了解底层网络协议
- [grpc][]
- [thrift][]

![rpc][]

# [微服务][micro_service]

- 将应用程序分解为一组松耦合的服务
- 服务间通过RESTful API及类似技术进行通信

# 本周作业

- 用ApiFox完成项目API的设计

[awesome rest]: https://github.com/marmelab/awesome-rest
[github api]: https://developer.github.com/v3/?
[grpc]: https://grpc.io/
[httpie]: https://github.com/jkbrzt/httpie
[json vs xml]: https://restfulapi.net/json-vs-xml/
[json]: http://www.json.org/
[micro_service]: https://github.com/mfornos/awesome-microservices
[postman]: https://chrome.google.com/webstore/detail/postman-rest-client/fdmmgilgnpjigdojojpjoooidkmcomcm
[rest_best_practice]: https://www.vinaysahni.com/best-practices-for-a-pragmatic-restful-api
[rest_best_practice_cn]: https://www.oschina.net/translate/best-practices-for-a-pragmatic-restful-api
[rest_cs]: ./rest_cs.png "RESTful Architecture"
[rest_guide]: http://www.ruanyifeng.com/blog/2014/05/restful_api.html
[rest_img]: ./rest.png "RESTful API"
[rest_paper]: https://www.ics.uci.edu/~fielding/pubs/dissertation/top.htm
[rpc]: ./rpc.jpg "RPC"
[ruan]: http://www.ruanyifeng.com/blog/2011/09/restful.html
[thrift]: https://thrift.apache.org/
[xml]: https://www.w3.org/XML/
