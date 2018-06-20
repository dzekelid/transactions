---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Operations/unsignedTransactions:
    get:
      summary: Get API Operations Unsignedtransactions
      description: Get api operations unsignedtransactions.
      operationId: ApiOperationsUnsignedTransactionsGet
      x-api-path-slug: apioperationsunsignedtransactions-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Unsignedtransactions
    post:
      summary: Add API Operations Unsignedtransactions
      description: Add api operations unsignedtransactions.
      operationId: ApiOperationsUnsignedTransactionsPost
      x-api-path-slug: apioperationsunsignedtransactions-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Unsignedtransactions
  /api/Transactions:
    get:
      summary: Get API Transactions
      description: Get api transactions.
      operationId: ApiTransactionsGet
      x-api-path-slug: apitransactions-get
      parameters:
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Transactions
---