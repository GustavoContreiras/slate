# Stock Exchanges

## Get stock exchange data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/stock_exchanges/?stock=ibovespa&limit=2", {
  "method": "GET",
  "headers": {}
})
.then(response => { console.log(response); })
.catch(err => { console.error(err); });
```

> Exemplo Resposta

```json
[
  {
    "date": "2021-03-19",
    "time": "00:00:00",
    "stock": "DJI       ",
    "open": 32858.36,
    "high": 32858.36,
    "low": 32505.07,
    "close": 32627.97,
    "adjClose": 32627.97,
    "volume": 8118
  },
  {
    "date": "2021-03-18",
    "time": "00:00:00",
    "stock": "DJI       ",
    "open": 32928.16,
    "high": 33227.78,
    "low": 32831.25,
    "close": 32862.3,
    "adjClose": 32862.3,
    "volume": 4184
  }
]
```

This endpoint retrieves stock exchanges data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
stock | null | Can be **dji**, **ibovespa**, **nikkei_225**, **sep_500** and **sse**.
limit | null | How many results should be returned. If null returns all.