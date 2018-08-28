---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 0
info:
  title: Neblio Get transactions by block or address
  description: Returns all transactions by block or address
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ins/txs:
    get:
      summary: Get transactions by block or address
      description: Returns all transactions by block or address
      operationId: getTxs
      x-api-path-slug: instxs-get
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: block
        description: Block Hash
      - in: query
        name: pageNum
        description: Page number to display
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - By
      - Block
      - Address
  /testnet/ins/txs:
    get:
      summary: Get transactions by block or address
      description: Returns all transactions by block or address
      operationId: testnet_getTxs
      x-api-path-slug: testnetinstxs-get
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: block
        description: Block Hash
      - in: query
        name: pageNum
        description: Page number to display
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - By
      - Block
      - Address
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