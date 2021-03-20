# PIB Monitors

## Get pib monitor data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/pib_monitors/?country=brazil&limit=2", {
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
    "country": "Brasil",
    "date": "2021-03-03",
    "period": "4 trim. 2020",
    "actual": 3.2,
    "forecast": 7,
    "previous": 7.7
  },
  {
    "country": "Brasil",
    "date": "2020-12-03",
    "period": "3 trim. 2020",
    "actual": 7.7,
    "forecast": -10.4,
    "previous": -9.7
  }
]
```

This endpoint retrieves pib monitors data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
country | null | Can be **brazil**, **usa**, **china**, **germany**, **australia**, **europe**, **south_africa**, **japan**, **united_kingdom** and **hong_kong**.
limit | null | How many results should be returned. If null returns all.