---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 0
info:
  title: RipaEx Peer Transactions From Ids
  description: Get a list of transactions by ids.
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/transactions/get:
    get:
      summary: Transactions Get
      description: Get a single transaction.
      operationId: transactions.getTransaction
      x-api-path-slug: apitransactionsget-get
      parameters:
      - in: query
        name: id
        description: A valid transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
  /api/transactions:
    get:
      summary: Transactions
      description: Get all transactions.
      operationId: transactions.getTransactions
      x-api-path-slug: apitransactions-get
      parameters:
      - in: query
        name: amount
        description: An unsigned integer that specifies the transaction amount
      - in: query
        name: blockId
        description: An unsigned integer that specifies the block ID
      - in: query
        name: fee
        description: An unsigned integer that specifies the transaction fee
      - in: query
        name: limit
        description: An unsigned integer that specifies the maximum number of records
      - in: query
        name: offset
        description: An unsigned integer that specified the number of records to skip
      - in: query
        name: orderBy
        description: A string that specifies the column by which to sort the records
      - in: query
        name: ownerAddress
        description: A valid RIPA Address
      - in: query
        name: ownerPublicKey
        description: A valid RIPA Address
      - in: query
        name: recipientId
        description: A valid RIPA Address
      - in: query
        name: senderId
        description: A valid RIPA Address
      - in: query
        name: senderPublicKey
        description: A valid RIPA Public Key
      - in: query
        name: type
        description: An unsigned integer that specifies the transaction type
      - in: query
        name: vendorField
        description: A string that specifies the SmartBridge used
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
    put:
      summary: Transactions
      description: Create a new transaction.
      operationId: transactions.addTransactions
      x-api-path-slug: apitransactions-put
      parameters:
      - in: body
        name: body
        description: A valid transaction object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
  /api/transactions/unconfirmed/get:
    get:
      summary: Transactions Unconfirmed Get
      description: Get a single unconfirmed transaction.
      operationId: transactions.getUnconfirmedTransaction
      x-api-path-slug: apitransactionsunconfirmedget-get
      parameters:
      - in: query
        name: id
        description: A valid unconfirmed transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - Unconfirmed
  /api/transactions/unconfirmed:
    get:
      summary: Transactions Unconfirmed
      description: Get all unconfirmed transactions.
      operationId: transactions.getUnconfirmedTransactions
      x-api-path-slug: apitransactionsunconfirmed-get
      parameters:
      - in: query
        name: address
        description: A valid RIPA Address
      - in: query
        name: senderPublicKey
        description: A valid RIPA Public Key
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - Unconfirmed
  /peer/transactions:
    get:
      summary: Peer Transactions
      description: .
      operationId: transport.getTransactions
      x-api-path-slug: peertransactions-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Peer
      - Transactions
    post:
      summary: Peer Transactions
      description: Create a new transaction.
      operationId: transport.addTransactions
      x-api-path-slug: peertransactions-post
      parameters:
      - in: body
        name: transactions
        description: A valid transaction object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Peer
      - Transactions
  /peer/transactionsFromIds:
    get:
      summary: Peer Transactions From Ids
      description: Get a list of transactions by ids.
      operationId: transport.transactionsFromIds
      x-api-path-slug: peertransactionsfromids-get
      parameters:
      - in: query
        name: ids
        description: A list of transaction IDs
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Peer
      - Transactions
      - From
      - Ids
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