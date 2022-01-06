# API de discos utilizando Go

Estudos utilizando Go para criação da API explicada na página oficial: https://go.dev/doc/tutorial/web-service-gin

## Stack
- Go
- Gin (https://github.com/gin-gonic/gin)

## Requisições utilizando cURL
get:: /albums
```
curl --location --request GET 'http://localhost:8080/albums'
```

get:: /albums/id
```
curl --location --request GET 'http://localhost:8080/albums/1'
```

post:: /albums
```
curl --location --request POST 'http://localhost:8080/albums' \
--header 'Content-Type: application/json' \
--data-raw '{
        "id": "5",
        "title": "Beg for Mercy",
        "artist": "G-Unit",
        "price": 9.99
    }'
```

As collections em formato json para serem utilizadas no Postman estão no diretório *json-collection*.