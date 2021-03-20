# ICS & ICR

## Get ics & icr data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/ics_icr/?type=ics&limit=2", {
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
    "date": "2021-03-04",
    "type": "ics",
    "estabelecimento": 99.1633561908453,
    "estabelecimentoImpact": 0.6334891384894625,
    "volume": 78.8166049306892,
    "volumeImpact": -20.25847206485667,
    "valor": 90.8975498433553,
    "valorImpact": -12.26485275280212
  },
  {
    "date": "2021-03-03",
    "type": "ics",
    "estabelecimento": 99.1633561908453,
    "estabelecimentoImpact": 0.6334891384894625,
    "volume": 78.8166049306892,
    "volumeImpact": -20.25847206485667,
    "valor": 90.8975498433553,
    "valorImpact": -12.26485275280212
  }
]
```

This endpoint retrieves ICS & ICR data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
type | null | Can be **ics** and **icr**.
limit | null | How many results should be returned. If null returns all.