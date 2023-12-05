# fullcycle-broker

Projeto criado durante imersão FullCycle utilizando Go, Apache Kafka, NestJs e NextJs

## broker

Projeto em Go que irá representar o mercado de ações realizando ações de compra e venda de ordens do mercado de ações.

## kafka

Acesse http://localhost:9021/ após o docker-compose up para publicar/ler mensagem kafka

Exemplo de mensagem de venda: 

`{
  "order_id": "1",
  "investor_id": "Mari",
  "asset_id": "asset1",
  "current_shares": 10,
  "shares": 5,
  "price": 5.0,
  "order_type": "SELL"
}`

Exemplo de mensagem de compra:

`{
  "investor_id": "Celia",
  "asset_id": "asset1",
  "current_shares": 0,
  "shares": 5,
  "price": 5.0,
  "order_type": "BUY"
}`

## nestjs-microservice

## nextjs-frontend