# Authentication

> Exemplo Request

```xml
GET https://www.plataformago.dragonflyinteligencia.com/indicators/metals/
Host: api.feegow.com/v1
Content-Type: application/json
x-access-token: "SEUTOKEN";
```

> Exemplo Parâmetros

```json
{
	country: "brazil"
}
	
```

> Exemplo Resposta

```
oi
```

Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>