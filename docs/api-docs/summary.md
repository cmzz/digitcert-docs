---
weight: 1
bookFlatSection: true
title: "概述"
---

# 概述

DigitCert 是专业的 SSL 提供商, 随着有开发能力客户的诉求, 和合作伙伴的呼吁, 我们隆重推出完整功能的接口 API.

## 环境

- https://www.digitcert.com.cn/api 正式环境, 合作伙伴/代理商应选择正式环境接入线上业务。
- 测试环境搭建中...

## 签名
API 采取 sha256 摘要签名, 在具体业务调用中, 只请求 `access_key`, 而机密的 `access_secret` 不出现在互联网中, 提升安全性。
具体签名算法介绍请见 [这里](/docs/api-docs/signature/).

## SDK 和模块插件
我们目前提供了常用系统的模组和 PHP 的 SDK, 也欢迎开源社区提供其他系统的 SDK 和模组, 一经采用可获 300 ~ 1000 元奖励。
