# Requisicao de dados Api-Criptomoedas
Requisição de dados de uma API de criptomoedas

#### Criação de conta no CoinMarketCap
https://pro.coinmarketcap.com/account

Vai precisar copiar a key da API para fazer a requisição.

```js
var apikey = {
    key: ''
}

if (apikey.key == "") {
    apikey.key = prompt("Digite a Key da API:");
}
```
No código acima foi implementado uma condicional com um prompt para inserir a key.

#### Front-end com Bootstrap
Foi utilizado o BootstrapCDN com o link direto.

```html
<link rel="stylesheet" type="text/css" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css">
```

#### Implementação do first_historical_data

```html
<div class="media">
    <img src="coin.jpg" class="align-self-center mr-3" alt="coin" width="100" height="60">
    <div class="media-body">
        <h5 class="mt-2">${api.data[i].name}</h5>
        <p>${api.data[i].symbol} - ${api.data[i].first_historical_data}</p>
    </div>
</div>  
```