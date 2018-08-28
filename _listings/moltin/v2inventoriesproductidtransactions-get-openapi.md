---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Stock transactions for a product
  description: Stock transactions for a product.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/inventories/{productID}/transactions:
    get:
      summary: Stock transactions for a product
      description: Stock transactions for a product.
      operationId: V2InventoriesTransactionsByProductIDGet
      x-api-path-slug: v2inventoriesproductidtransactions-get
      parameters:
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Stock
      - Transactionsa
      - Products
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