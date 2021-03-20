# ICVA

## Get icva data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/icva/limit=2", {
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
    "nominal": -9.9,
    "nominalAdjusted": -7.199999999999999,
    "deflated": -17.1,
    "deflatedAdjusted": -12.1
  },
  {
    "date": "2021-01-01",
    "nominal": -6.3,
    "nominalAdjusted": -3.9,
    "deflated": -12.6,
    "deflatedAdjusted": -10.3
  }
]
```

This endpoint retrieves coffees data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
limit | null | How many results should be returned. If null returns all.