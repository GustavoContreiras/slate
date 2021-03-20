# Coffees

## Get coffee data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/coffees/?coffee=robusta&limit=2", {
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
    "date": "2021-02-05",
    "real": 424.72,
    "dollar": 78.86
  },
  {
    "date": "2021-02-04",
    "real": 425.91,
    "dollar": 78.09
  }
]
```

This endpoint retrieves coffees data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
coffee | null | Can be **arabica** and **robusta**.
limit | null | How many results should be returned. If null returns all.