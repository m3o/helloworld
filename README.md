# Helloworld

This is a simple Go app which returns helloworld.

## Usage

Run it
```
go run main.go
```

Call it
```
curl http://localhost:8080?name=Alice
```

Get JSON

```
curl -H 'Content-Type: application/json` -d '{"name": "Alice"}' http://localhost:8080
```
