# Grok Imagine 2.0 API (grok-imagine-2.0 / grokimagine2.0) — api guide with published pricing

> **upload-image $0; default $0.015; region-edit $0.015** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-d1e20e)** · **[Get an API key](https://go.apimart.ai/k-a35bac)**

Everything here refers to **grok-imagine-2.0** — also written **grokimagine2.0** or **grok imagine 2.0**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `upload-image` | $0 |
| `default` | $0.015 |
| `region-edit` | $0.015 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $0 |
| 1,000 | $0 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"grok-imagine-2.0-ext","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
