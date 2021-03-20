# IPCA

## Get IPCA data

> Exemplo Request

```javascript
fetch("https://www.plataformago.dragonflyinteligencia.com/indicators/ipca/?category=indice_geral&limit=2", {
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
    "year": 2021,
    "month": 2,
    "category": "Índice Geral",
    "monthVariation": 0.86,
    "yearVariation": 1.11,
    "monthWeight": 100
  },
  {
    "year": 2021,
    "month": 1,
    "category": "Índice Geral",
    "monthVariation": 0.25,
    "yearVariation": 0.25,
    "monthWeight": 100
  }
]
```

This endpoint retrieves IPCA data.

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
category | null | Can be **indice_geral**, **alimentacao_e_bebidas**, **artigos_de_residencia**, **comunicacao**, **despesas_pessoais**, **educacao**, **habitacao**, **saude_e_cuidados_pessoais**, **transportes**, and **vestuario**.
limit | null | How many results should be returned. If null returns all.