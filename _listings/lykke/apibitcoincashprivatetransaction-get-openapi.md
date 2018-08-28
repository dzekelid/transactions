---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API Bitcoincash Private Transaction
  version: 1.0.0
  description: Get api bitcoincash private transaction.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
  /api/BitcoinCash/multisig/transaction:
    get:
      summary: Get API Bitcoincash Multisig Transaction
      description: Get api bitcoincash multisig transaction.
      operationId: ApiBitcoinCashMultisigTransactionGet
      x-api-path-slug: apibitcoincashmultisigtransaction-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: destinationAddress
      responses:
        200:
          description: OK
      tags:
      - Bitcoincash
      - Multisig
      - Transaction
  /api/BitcoinCash/private/transaction:
    get:
      summary: Get API Bitcoincash Private Transaction
      description: Get api bitcoincash private transaction.
      operationId: ApiBitcoinCashPrivateTransactionGet
      x-api-path-slug: apibitcoincashprivatetransaction-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: destinationAddress
      - in: query
        name: fee
      - in: query
        name: sourceAddress
      responses:
        200:
          description: OK
      tags:
      - Bitcoincash
      - Private
      - Transaction
  /api/BcnTransaction:
    get:
      summary: Get API Bcntransaction
      description: Get api bcntransaction.
      operationId: ApiBcnTransactionGet
      x-api-path-slug: apibcntransaction-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransaction
  /api/BcnTransaction/offchain-trade:
    get:
      summary: Get API Bcntransaction Offchain Trade
      description: Get api bcntransaction offchain trade.
      operationId: ApiBcnTransactionOffchain-tradeGet
      x-api-path-slug: apibcntransactionoffchaintrade-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransaction
      - Offchain
      - Trade
  /api/BcnTransactionByCashOperation/{id}:
    get:
      summary: Get API Bcntransactionbycashoperation
      description: Get api bcntransactionbycashoperation.
      operationId: ApiBcnTransactionByCashOperationByIdGet
      x-api-path-slug: apibcntransactionbycashoperationid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransactionbycashoperation
  /api/BcnTransactionByExchange/{id}:
    get:
      summary: Get API Bcntransactionbyexchange
      description: Get api bcntransactionbyexchange.
      operationId: ApiBcnTransactionByExchangeByIdGet
      x-api-path-slug: apibcntransactionbyexchangeid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransactionbyexchange
  /api/BcnTransactionByTransfer/{id}:
    get:
      summary: Get API Bcntransactionbytransfer
      description: Get api bcntransactionbytransfer.
      operationId: ApiBcnTransactionByTransferByIdGet
      x-api-path-slug: apibcntransactionbytransferid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransactionbytransfer
  /api/BlockchainTransaction:
    get:
      summary: Get API Blockchaintransaction
      description: Get api blockchaintransaction.
      operationId: ApiBlockchainTransactionGet
      x-api-path-slug: apiblockchaintransaction-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: blockChainHash
      responses:
        200:
          description: OK
      tags:
      - Blockchaintransaction
  /api/BroadcastTransaction:
    post:
      summary: Add API Broadcasttransaction
      description: Add api broadcasttransaction.
      operationId: ApiBroadcastTransactionPost
      x-api-path-slug: apibroadcasttransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Broadcasttransaction
  /api/Ethereum/privateWallet/broadcastTransaction:
    post:
      summary: Add API Ethereum Privatewallet Broadcasttransaction
      description: Add api ethereum privatewallet broadcasttransaction.
      operationId: ApiEthereumPrivateWalletBroadcastTransactionPost
      x-api-path-slug: apiethereumprivatewalletbroadcasttransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Privatewallet
      - Broadcasttransaction
  /api/Ethereum/privateWallet/estimateTransaction:
    post:
      summary: Add API Ethereum Privatewallet Estimatetransaction
      description: Add api ethereum privatewallet estimatetransaction.
      operationId: ApiEthereumPrivateWalletEstimateTransactionPost
      x-api-path-slug: apiethereumprivatewalletestimatetransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Privatewallet
      - Estimatetransaction
  /api/Ethereum/privateWallet/generateTransaction:
    post:
      summary: Add API Ethereum Privatewallet Generatetransaction
      description: Add api ethereum privatewallet generatetransaction.
      operationId: ApiEthereumPrivateWalletGenerateTransactionPost
      x-api-path-slug: apiethereumprivatewalletgeneratetransaction-post
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
      - Ethereum
      - Privatewallet
      - Generatetransaction
  /api/Ethereum/tx/{transactionHash}:
    get:
      summary: Get API Ethereum Tx Transactionhash
      description: Get api ethereum tx transactionhash.
      operationId: ApiEthereumTxByTransactionHashGet
      x-api-path-slug: apiethereumtxtransactionhash-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: transactionHash
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Tx
      - Transactionhash
  /api/GenerateTransferTransaction:
    post:
      summary: Add API Generatetransfertransaction
      description: Add api generatetransfertransaction.
      operationId: ApiGenerateTransferTransactionPost
      x-api-path-slug: apigeneratetransfertransaction-post
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
      - Generatetransfertransaction
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