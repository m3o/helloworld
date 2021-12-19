# Helloworld

This is a simple helloworld app powered by [m3o.com](https://m3o.com).

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
