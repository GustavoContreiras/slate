# Savings Report

## Get savings report data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/savings_report/?limit=2", {
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
    "date": "2021-03-05",
    "deposit": 19799674,
    "withdraw": 14751008,
    "netCapital": 5048666,
    "yield": 67806,
    "balance": 1023766185
  },
  {
    "date": "2021-03-04",
    "deposit": 12579733,
    "withdraw": 10710888,
    "netCapital": 1868845,
    "yield": 67904,
    "balance": 1018649712
  }
]
```

This endpoint retrieves savings report data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
limit | null | How many results should be returned. If null returns all.