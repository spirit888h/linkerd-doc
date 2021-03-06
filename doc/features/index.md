# 特性

除了通过熔断和延迟感知负载均衡增加可靠性外，Linkerd还自动展示顶级服务指标，如请求量，成功率和延迟分布。Linkerd 还通过被称为 dtabs 的强大语言提供了请求级路由和多服务发现集成。

在本节中，您将找到 linkerd 的主要功能。

- [负载平衡](load-balancing.md)：linkerd提供了多种负载均衡算法，它们使用实时性能指标来分配负载并减少整个应用程序的尾部延迟。

- [熔断](circuit-breaking.md)：linkerd包含自动熔断，将停止将流量发送到被认为不健康的实例，从而使他们有机会恢复并避免连锁反应故障。

- [服务发现](service-discovery.md)：linkerd 与各种服务发现后端集成，通过删除特定的(ad-hoc)服务发现实现来帮助您降低代码的复杂性。

- [动态请求路由](routing.md)：linkerd 启用动态请求路由和重新路由，允许您使用最少量的配置来设置分段服务(staging service)，金丝雀(canaries)，蓝绿部署(blue-green deploy)，跨DC故障切换和黑暗流量(dark traffic)。

- [重试次数和截止日期](retries-deadlines.md)：linkerd可以在某些故障时自动重试请求，并且可以在指定的时间段之后让请求超时。

- [TLS](tls.md)：linkerd 可以配置为使用 TLS 发送和接收请求，您可以使用它来加密跨主机边界的通信，而不用修改现有的应用程序代码。

- [HTTP代理集成](http-proxy.md)：linkerd 可以作为 HTTP 代理，几乎所有现代 HTTP 客户端都广泛支持，使其易于集成到现有应用程序中。

- [透明代理](transparent-proxying.md)：您可以在主机上使用 iptables 规则，设置通过 linkerd 的透明代理

- [gRPC](grpc.md)：linkerd 支持 HTTP/2 和 TLS，允许它路由 gRPC 请求，支持高级 RPC 机制，如双向流，流程控制和结构化数据负载。

- [分布式跟踪](distributed-tracing-and-instrumentation.md)：linkerd 支持分布式跟踪和度量仪器，可以提供跨越所有服务的统一的可观察性。

- [仪器仪表](instrumentation.md): linkerd 支持分布式跟踪和度量仪器，可以提供跨越所有服务的统一的可观察性。