---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Get Receipts Receipt Transactions
  description: Retrieves a set of Transaction objects associated to a Receipt.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /receipts/{receipt_id}/transactions:
    get:
      summary: Get Receipts Receipt Transactions
      description: Retrieves a set of Transaction objects associated to a Receipt.
      operationId: getReceiptsReceiptTransactions
      x-api-path-slug: receiptsreceipt-idtransactions-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: receipt_id
      responses:
        200:
          description: OK
      tags:
      - Receipts
      - Receipt
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