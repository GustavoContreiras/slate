# Metals

## Get metal data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/metals/?metal=gold&limit=2", {
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
    "date": "2021-03-20",
    "time": "07:44:00",
    "open": null,
    "close": 1749.6,
    "high": null,
    "low": null
  },
  {
    "date": "2021-03-19",
    "time": "12:00:00",
    "open": null,
    "close": 1749.6,
    "high": null,
    "low": null
  }
]
```

This endpoint retrieves metals data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
metal | null | Can be **gold**, **silver**, **copper**, **platinum**, **palladium** and **iron**.
limit | null | How many results should be returned. If null returns all.