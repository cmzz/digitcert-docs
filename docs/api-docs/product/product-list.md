---
weight: 3
bookFlatSection: true
title: "产品列表"
---

# 产品列表

获取平台在售产品列表。


## 请求

- 主机：dev.digitalcert.test
- 接口：/api/v1/products
- 动作：GET
    
    ### example
    ```http request
    GET /api/v1/products HTTP/1.1
    Content-Type: application/json
    Accept: application/json
    Cache-Control: no-cache
    Host: dev.digitalcert.test
    ```

## 响应

- `id`: 证书id
- `brand_id`: 品牌id
- `title`: 产品名称
- `san_enabled`: 是否支持san
- `multi_domain`: 是否支持多域名
- `san_max`: 最大san数量
- `san_included`: 默认包含san数量
- `prices.period`: 周期
- `prices.cost.price`: 成本价
- `prices.cost.san_price`: san成本价
- `prices.retail_price.price`: 零售价
- `prices.retail_price.san_price`: san零售价

    ### example
    ```json
    [
        {
            "id": 1,
            "brand_id": 12,
            "title": "扩展 EV 证书",
            "san_enabled": 0,
            "multi_domain": 0,
            "san_included": 0,
            "san_max": "0",
            "prices": [
                {
                    "period": 12,
                    "cost": {
                        "price": "699.00",
                        "san_price": "0.00"
                    },
                    "retail_price": {
                        "price": "1688.00",
                        "san_price": "0.00"
                    }
                },
                {
                    "period": 24,
                    "cost": {
                        "price": "1328.00",
                        "san_price": "0.00"
                    },
                    "retail_price": {
                        "price": "3098.00",
                        "san_price": "0.00"
                    }
                }
            ]
        },
    ]
    ```
    

