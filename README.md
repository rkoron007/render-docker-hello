# render-docker-hello

A minimal Docker web service for Render. It serves a plain-text greeting on the port in `$PORT`.

## Deploy on Render

1. In the [Render Dashboard](https://dashboard.render.com), click **New > Web Service** and connect this repo.
2. Set **Language** to **Docker**. Render builds the `Dockerfile` at the repo root.
3. Click **Deploy Web Service**.

## Run locally

```bash
docker build -t render-docker-hello .
docker run --rm -p 10000:10000 render-docker-hello
curl localhost:10000
```
