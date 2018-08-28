---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List payments of a transaction type
  description: Lists all payments of a transaction type. The ID of the transaction
    type must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/orders/items/{orderItemId}/transactions:
    get:
      summary: List transactions
      description: Lists transactions for an order item. The ID of the order item
        must be specified.
      operationId: getRestOrdersItemsOrderitemTransactions
      x-api-path-slug: restordersitemsorderitemidtransactions-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: orderItemId
      - in: query
        name: with
        description: Load additional relations for a transaction
      responses:
        200:
          description: OK
      tags:
      - List
      - Transactions
    post:
      summary: Create a transaction
      description: Create a transaction.
      operationId: postRestOrdersItemsOrderitemTransactions
      x-api-path-slug: restordersitemsorderitemidtransactions-post
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /rest/payments/transactions/{transactionTypeId}:
    get:
      summary: List payments of a transaction type
      description: Lists all payments of a transaction type. The ID of the transaction
        type must be specified.
      operationId: getRestPaymentsTransactionsTransactiontype
      x-api-path-slug: restpaymentstransactionstransactiontypeid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: transactionTypeId
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Transaction
      - Type
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