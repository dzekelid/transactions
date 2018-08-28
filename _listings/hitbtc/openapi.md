swagger: "2.0"
x-collection-name: HitBTC
x-complete: 1
info:
  title: HitBTC API
  description: create-api-keys-in-your-profile-httpshitbtc-comsettingsapikeys-and-use-public-api-key-as-username-and-secret-as-password-to-authorize-
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/transactions:
    get:
      summary: Get Account Transactions
      description: Get account transactions.
      operationId: getAccountTransactions
      x-api-path-slug: accounttransactions-get
      parameters:
      - in: query
        name: by
        description: Filter field
      - in: query
        name: currency
      - in: query
        name: from
        description: Datetime in iso format or timestamp in millisecond, or index
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: sort
        description: Sort direction
      - in: query
        name: till
        description: Datetime in iso format or timestamp in millisecond, or index
      responses:
        200:
          description: OK
      tags:
      - Account
      - Transactions
  /account/transactions/{id}:
    get:
      summary: Get Account Transaction By Id
      description: Get account transaction by id.
      operationId: getAccountTransactions
      x-api-path-slug: accounttransactionsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Account
      - Transaction
      - By
      - Id