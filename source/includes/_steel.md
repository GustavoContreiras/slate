# Steel

## Get steel data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/steel/?limit=2", {
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
    "date": "2021-02-01",
    "production": 7700523,
    "domesticSales": 1882947,
    "foreignMarket": 657043,
    "exports": 765572,
    "imports": 333870,
    "apparentConsumption": 2125371
  },
  {
    "date": "2021-01-01",
    "production": 8220748,
    "domesticSales": 1923804,
    "foreignMarket": 565529,
    "exports": 531149,
    "imports": 324474,
    "apparentConsumption": 2211070
  }
]
```

This endpoint retrieves steel data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
limit | null | How many results should be returned. If null returns all.