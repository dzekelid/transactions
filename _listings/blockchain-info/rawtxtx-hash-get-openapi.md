---
swagger: "2.0"
x-collection-name: Blockchain Info
x-complete: 0
info:
  title: Blockchain Info Raw Transaction
  description: Returns a raw trasaction.
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rawtx/{tx_hash}:
    get:
      summary: Raw Transaction
      description: Returns a raw trasaction.
      operationId: getRawTransaction
      x-api-path-slug: rawtxtx-hash-get
      parameters:
      - in: query
        name: tx_hash
        description: The hash
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---