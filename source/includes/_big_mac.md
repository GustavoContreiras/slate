# Big Mac Index

## Get big mac index data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/big_mac/?country=brazil&limit=2", {
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
    "date": "2021-01-01T00:00:00",
    "countryCode": "BRA",
    "currencyCode": "BRL",
    "countryName": "Brazil",
    "localPrice": 21.9,
    "dollarEx": 5.5046,
    "dollarPrice": 3.97849071685499,
    "usdRaw": -0.29709,
    "eurRaw": -0.22957,
    "gbpRaw": -0.10348,
    "jpyRaw": 0.06394,
    "cnyRaw": 0.15005,
    "gdpDollar": 8751.381,
    "adjustedPrice": 3.21778192537769,
    "usdAdjusted": 0.20101,
    "eurAdjusted": 0.06636,
    "gbpAdjusted": 0.27461,
    "jpyAdjusted": 0.48431,
    "cnyAdjusted": 0.17219
  },
  {
    "date": "2020-07-01T00:00:00",
    "countryCode": "BRA",
    "currencyCode": "BRL",
    "countryName": "Brazil",
    "localPrice": 20.9,
    "dollarEx": 5.34045,
    "dollarPrice": 3.91352788622682,
    "usdRaw": -0.31462,
    "eurRaw": -0.18232,
    "gbpRaw": -0.08505,
    "jpyRaw": 0.07647,
    "cnyRaw": 0.26306,
    "gdpDollar": 8958.576,
    "adjustedPrice": 2.97800388981275,
    "usdAdjusted": 0.1909,
    "eurAdjusted": 0.16771,
    "gbpAdjusted": 0.33581,
    "jpyAdjusted": 0.52339,
    "cnyAdjusted": 0.2738
  }
]
```

This endpoint retrieves big mac index data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
country | null | Can be **brazil**, **usa**, **china**, **australia**, **europe**, **india**, **japan**, **russia** and **hong_kong**.
limit | null | How many results should be returned. If null returns all.