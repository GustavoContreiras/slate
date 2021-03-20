# Oils

## Get oil data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/oils/?oil=brent&limit=2", {
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
    "date": "2021-03-19T00:00:00",
    "oil": "brent",
    "open": 62.83,
    "high": 64.9,
    "low": 62.08,
    "close": 64.53,
    "volume": 61688
  },
  {
    "date": "2021-03-18T00:00:00",
    "oil": "brent",
    "open": 67.93,
    "high": 68.15,
    "low": 61.42,
    "close": 63.28,
    "volume": 61688
  }
]
```

This endpoint retrieves oils data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
oil | null | Can be **brent** and **crude**.
limit | null | How many results should be returned. If null returns all.