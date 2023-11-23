# web-service-gin
RESTful API with GO and Gin

To start the application
```
go run .
```

## GET /albums
To get all albums
```
curl http://localhost:8080/albums
```

## POST albums
To add an album
```
curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```

## GET albums/{id}
To get album by ID
```
curl http://localhost:8080/albums/2
```