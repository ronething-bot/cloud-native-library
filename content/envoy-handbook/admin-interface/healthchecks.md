---
weight: 80
title: 健康检查
date: '2022-05-18T00:00:00+08:00'
type: book
---

`/healthcheck/fail` 可用于失败的入站健康检查。端点 `/healthcheck/ok` 用于恢复失败的端点。

这两个端点都需要使用 HTTP 健康检查过滤器。我们可能会在关闭服务器前或进行完全重启时使用它来排空服务器。当调用失败的健康检查选项时，所有的健康检查都将失败，无论其配置如何。