# Helloworld

This is helloworld powered by [M3O](https://m3o.com).

## Usage

Run it using the [M3O Apps](https://m3o.com/app) service.

### Cloud

Use M3O Cloud at [cloud.m3o.com](https://cloud.m3o.com)

### CLI

```
m3o app run --name=helloworld --repo=github.com/m3o/helloworld
```

Get an app url back. In this case `helloworld.m3o.app`.

```bash
curl https://helloworld.m3o.app?name=Alice
```

### API

```
curl "https://api.m3o.com/v1/app/Run" \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer $M3O_API_TOKEN" \
  -d '{
    "branch": "master",
    "name": "helloworld",
    "port": 8080,
    "region": "europe-west1",
    "repo": "github.com/m3o/helloworld"
  }'
```
