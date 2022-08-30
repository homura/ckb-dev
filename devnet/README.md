# Integration via Docker

A docker-compose to launch a local ckb + ckb-indexer with 1s/block and 2s/epoch

## Quick Start

```sh
docker compose up
# docker compose up --build
# docker compose up --detach
```

```sh
curl --request POST 'http://localhost:8114' \
--header 'Content-Type: application/json' \
--data-raw '{
  "id": 42,
  "jsonrpc": "2.0",
  "method": "get_tip_block_number"
}'
```

## Troubleshooting

### ckb-cli Cannot Access Local CKB Node

If you have a proxy on, try turning it off and try again
