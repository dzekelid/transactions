---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 1
info:
  title: Etsy
  description: bring-etsys-handmade-marketplace-and-community-into-your-apps-
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
  /shops/{shop_id}/transactions:
    get:
      summary: Get Shops Shop Transactions
      description: Retrieves a set of Transaction objects associated to a Shop.
      operationId: getShopsShopTransactions
      x-api-path-slug: shopsshop-idtransactions-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: shop_id
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Transactions
  /transactions/{transaction_id}:
    get:
      summary: Get Transactions Transaction
      description: Retrieves a Transaction by id.
      operationId: getTransactionsTransaction
      x-api-path-slug: transactionstransaction-id-get
      parameters:
      - in: path
        name: transaction_id
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Transaction
  /users/{user_id}/transactions:
    get:
      summary: Get Users User Transactions
      description: Retrieves a set of Transaction objects associated to a User.
      operationId: getUsersUserTransactions
      x-api-path-slug: usersuser-idtransactions-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Transactions
---