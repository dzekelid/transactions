swagger: "2.0"
x-collection-name: 3dcart
x-complete: 1
info:
  title: _3dCartWebAPI
  version: 1.0.0
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Orders/{orderid}/Transactions:
    get:
      summary: Gets the transactions from a specific Order
      description: Gets the transactions from a specific order.
      operationId: Orders_GetAllOrderTransactions
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Transactions
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of transactions from a specific Order
      description: Updates a collection of transactions from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transactions
        description: A Json or XML object containing the new transactions
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Transactions
      - From
      - Specific
      - Order
    post:
      summary: Adds a new transaction on the order
      description: Adds a new transaction on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transaction
        description: A Json or XML object containing the new transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Transaction
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Transactions/{transactionindexid}:
    put:
      summary: Updates a specific transaction from a specific Product
      description: Updates a specific transaction from a specific product.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactionstransactionindexid-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transaction
        description: A Json or XML object containing the new transaction
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: transactionindexid
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Transaction
      - From
      - Specific
      - Product