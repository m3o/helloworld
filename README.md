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

Get an app id back. In this case `helloworld`.

```bash
{
        "service": {
                "id": "helloworld",
                "name": "helloworld",
                "repo": "github.com/asim/helloworld",
                "branch": "master",
                "region": "europe-west1",
                "port": 8080,
                "status": "Running",
                "url": "https://helloworld.m3o.app",
                "created": "2021-12-15T09:48:50.864124234Z",
                "updated": "2021-12-16T20:54:19.532554Z",
                "env_vars": {},
                "custom_domains": []
        }
}
```

Call it via `[id].m3o.app`

```bash
curl https://helloworld.m3o.app?name=Alice
```

Get as JSON

```bash
curl -H 'Content-Type: application/json` \
    -d '{"name": "Alice"}' \
    https://helloworld.m3o.app
```
