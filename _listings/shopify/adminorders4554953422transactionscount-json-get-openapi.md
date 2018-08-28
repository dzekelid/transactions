---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get a count of transactions for an order
  description: Get a count of transactions for an order.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders/4554953422/transactions/count.json:
    get:
      summary: Get a count of transactions for an order
      description: Get a count of transactions for an order.
      operationId: getAdminOrders4554953422TransactionsCount.json
      x-api-path-slug: adminorders4554953422transactionscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Transactionsan
      - Order
  /admin/orders/4554953422/transactions.json:
    get:
      summary: Get all transactions for an order
      description: Get all transactions for an order.
      operationId: getAdminOrders4554953422Transactions.json
      x-api-path-slug: adminorders4554953422transactions-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Transactionsan
      - Order
  /admin/orders/4554953422/transactions/5016037966.json:
    get:
      summary: Get a specific transaction
      description: Get a specific transaction.
      operationId: getAdminOrders4554953422Transactions5016037966.json
      x-api-path-slug: adminorders4554953422transactions5016037966-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Specific
      - Transaction
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