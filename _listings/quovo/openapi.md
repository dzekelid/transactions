swagger: "2.0"
x-collection-name: Quovo
x-complete: 1
info:
  title: Quovo API v3
  description: todo-add-description
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
  /connections/{connection_id}/transactions:
    get:
      summary: Get a connection's transactions
      description: Provides information on a connection's historical transactions.
      operationId: ConnectionsTransactionsByConnectionIdGet
      x-api-path-slug: connectionsconnection-idtransactions-get
      parameters:
      - in: path
        name: connection_id
      responses:
        200:
          description: OK
      tags:
      - Connections
      - Transactions
  /accounts/{account_id}/transactions:
    get:
      summary: Get an account's transactions
      description: Provides information on an account's historical transactions.
      operationId: AccountsTransactionsByAccountIdGet
      x-api-path-slug: accountsaccount-idtransactions-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Transactions
  /users/{user_id}/transactions:
    get:
      summary: Get a user's transactions
      description: Provides historical transactions for a specific user.
      operationId: UsersTransactionsByUserIdGet
      x-api-path-slug: usersuser-idtransactions-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Transactions
  /transactions/{transaction_id}:
    get:
      summary: Get a single transaction
      description: Provides information on a single historical transaction.
      operationId: TransactionsByTransactionIdGet
      x-api-path-slug: transactionstransaction-id-get
      parameters:
      - in: path
        name: transaction_id
      responses:
        200:
          description: OK
      tags:
      - Single
      - Transaction
    put:
      summary: Update a transaction
      description: "Update an existing historical transaction. \n\nCurrently, only
        used to update a transaction's expense_category."
      operationId: TransactionsByTransactionIdPut
      x-api-path-slug: transactionstransaction-id-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: transaction_id
      responses:
        200:
          description: OK
      tags:
      - Transaction