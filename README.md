# Helloworld

This is a simple helloworld app powered by [m3o.com](https://m3o.com).

## Usage

Run it using the [App api](https://m3o.com/app).

```bash
curl "https://api.m3o.com/v1/app/Run" \
    -H "Content-Type: application/json" \
    -H "Authorization: Bearer $M3O_API_TOKEN" \
    -d '{
        "name": "helloworld",
        "repo": "github.com/asim/helloworld"
    }'
```

Get an app url back. In this case `helloworld.m3o.app`.

```bash
curl https://helloworld.m3o.app?name=Alice
```
