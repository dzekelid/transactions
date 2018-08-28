---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 0
info:
  title: Neblio Returns raw transaction hex
  description: Returns raw transaction hex representing a NEBL transaction
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ins/txs:
    get:
      summary: Get transactions by block or address
      description: Returns all transactions by block or address
      operationId: getTxs
      x-api-path-slug: instxs-get
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: block
        description: Block Hash
      - in: query
        name: pageNum
        description: Page number to display
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - By
      - Block
      - Address
  /testnet/ins/txs:
    get:
      summary: Get transactions by block or address
      description: Returns all transactions by block or address
      operationId: testnet_getTxs
      x-api-path-slug: testnetinstxs-get
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: block
        description: Block Hash
      - in: query
        name: pageNum
        description: Page number to display
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - By
      - Block
      - Address
  /ntp1/broadcast:
    post:
      summary: Broadcasts a signed raw transaction to the network
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: broadcastTx
      x-api-path-slug: ntp1broadcast-post
      parameters:
      - in: body
        name: body
        description: Object representing a transaction to broadcast
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Broadcasts
      - Signed
      - Raw
      - Transaction
      - To
      - Network
  /ntp1/transactioninfo/{txid}:
    get:
      summary: Information On an NTP1 Transaction
      description: Returns detailed information regarding an NTP1 transaction.
      operationId: getTransactionInfo
      x-api-path-slug: ntp1transactioninfotxid-get
      parameters:
      - in: path
        name: txid
        description: Neblio txid to get information on
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Information
      - "On"
      - NTP1
      - Transaction
  /ntp1/issue:
    post:
      summary: Builds a transaction that issues a new NTP1 Token
      description: Builds an unsigned raw transaction that issues a new NTP1 token
        on the Neblio blockchain.
      operationId: issueToken
      x-api-path-slug: ntp1issue-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Issues
      - New
      - NTP1
      - Token
  /ntp1/sendtoken:
    post:
      summary: Builds a transaction that sends an NTP1 Token
      description: Builds an unsigned raw transaction that sends an NTP1 token on
        the Neblio blockchain.
      operationId: sendToken
      x-api-path-slug: ntp1sendtoken-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be sent
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Sends
      - NTP1
      - Token
  /ntp1/burntoken:
    post:
      summary: Builds a transaction that burns an NTP1 Token
      description: Builds an unsigned raw transaction that burns an NTP1 token on
        the Neblio blockchain.
      operationId: burnToken
      x-api-path-slug: ntp1burntoken-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be burned
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Burns
      - NTP1
      - Token
  /ins/tx/send:
    post:
      summary: Broadcasts a signed raw transaction to the network (not NTP1 specific)
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: sendTx
      x-api-path-slug: instxsend-post
      parameters:
      - in: body
        name: body
        description: Object representing a transaction to broadcast
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Broadcasts
      - Signed
      - Raw
      - Transaction
      - To
      - Network
      - (not
      - NTP1
      - Specific)
  /ins/tx/{txid}:
    get:
      summary: Returns transaction object
      description: Returns NEBL transaction object representing a NEBL transaction
      operationId: getTx
      x-api-path-slug: instxtxid-get
      parameters:
      - in: path
        name: txid
        description: Transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Transaction
      - Object
  /ins/rawtx/{txid}:
    get:
      summary: Returns raw transaction hex
      description: Returns raw transaction hex representing a NEBL transaction
      operationId: getRawTx
      x-api-path-slug: insrawtxtxid-get
      parameters:
      - in: path
        name: txid
        description: Transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Raw
      - Transaction
      - Hex
  /testnet/ins/tx/send:
    post:
      summary: Broadcasts a signed raw transaction to the network (not NTP1 specific)
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: testnet_sendTx
      x-api-path-slug: testnetinstxsend-post
      parameters:
      - in: body
        name: body
        description: Object representing a transaction to broadcast
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Broadcasts
      - Signed
      - Raw
      - Transaction
      - To
      - Network
      - (not
      - NTP1
      - Specific)
  /testnet/ins/tx/{txid}:
    get:
      summary: Returns transaction object
      description: Returns NEBL transaction object representing a NEBL transaction
      operationId: testnet_getTx
      x-api-path-slug: testnetinstxtxid-get
      parameters:
      - in: path
        name: txid
        description: Transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Transaction
      - Object
  /testnet/ins/rawtx/{txid}:
    get:
      summary: Returns raw transaction hex
      description: Returns raw transaction hex representing a NEBL transaction
      operationId: testnet_getRawTx
      x-api-path-slug: testnetinsrawtxtxid-get
      parameters:
      - in: path
        name: txid
        description: Transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Raw
      - Transaction
      - Hex
  /testnet/ntp1/broadcast:
    post:
      summary: Broadcasts a signed raw transaction to the network
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: testnet_broadcastTx
      x-api-path-slug: testnetntp1broadcast-post
      parameters:
      - in: body
        name: body
        description: Object representing a transaction to broadcast
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Broadcasts
      - Signed
      - Raw
      - Transaction
      - To
      - Network
  /testnet/ntp1/transactioninfo/{txid}:
    get:
      summary: Information On an NTP1 Transaction
      description: Returns detailed information regarding an NTP1 transaction.
      operationId: testnet_getTransactionInfo
      x-api-path-slug: testnetntp1transactioninfotxid-get
      parameters:
      - in: path
        name: txid
        description: Neblio txid to get information on
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Information
      - "On"
      - NTP1
      - Transaction
  /testnet/ntp1/issue:
    post:
      summary: Builds a transaction that issues a new NTP1 Token
      description: Builds an unsigned raw transaction that issues a new NTP1 token
        on the Neblio blockchain.
      operationId: testnet_issueToken
      x-api-path-slug: testnetntp1issue-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Issues
      - New
      - NTP1
      - Token
  /testnet/ntp1/sendtoken:
    post:
      summary: Builds a transaction that sends an NTP1 Token
      description: Builds an unsigned raw transaction that sends an NTP1 token on
        the Neblio blockchain.
      operationId: testnet_sendToken
      x-api-path-slug: testnetntp1sendtoken-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be sent
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Sends
      - NTP1
      - Token
  /testnet/ntp1/burntoken:
    post:
      summary: Builds a transaction that burns an NTP1 Token
      description: Builds an unsigned raw transaction that burns an NTP1 token on
        the Neblio blockchain.
      operationId: testnet_burnToken
      x-api-path-slug: testnetntp1burntoken-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be burned
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Burns
      - NTP1
      - Token
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