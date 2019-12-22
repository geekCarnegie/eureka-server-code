# Eureka-Server
SpringCloud Eureka Server 注册中心<br>

## Eureka简介<br>
Eureka是Netflix开发的服务发现组件，本身是一个基于REST的服务。Spring Cloud将它集成在其子项目spring-cloud-netflix中，
以实现Spring Cloud的服务发现功能。Eureka现在已经从1.0升级到2.0，可惜的是Eureka2.0不在开源，但也不影响我们的使用。
由于基于REST服务，自然而然的就能想到，这个服务一定会有心跳检测、健康检查和客户端缓存等机制。

Eureka包括两个端：<br>
Eureka Server：注册中心服务端，用于维护和管理注册服务列表。<br>
Eureka Client：注册中心客户端，向注册中心注册服务的应用都可以叫做Eureka Client（包括Eureka Server本身）。

这里为Eureka Server端代码。