---
swagger: "2.0"
x-collection-name: Blockchain
x-complete: 1
info:
  title: Blockchain Info
  description: use-blockchains-apis-at-no-cost-to-help-you-start-building-bitcoin-apps-
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rawtx/{tx_hash}:
    get:
      summary: Raw Transaction
      description: Returns a raw trasaction.
      operationId: getRawTransaction
      x-api-path-slug: rawtxtx-hash-get
      parameters:
      - in: query
        name: tx_hash
        description: The hash
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
  /unconfirmed-transactions:
    get:
      summary: Unconfirmed Transactions
      description: Returns unconfirmed transactions.
      operationId: getUnconfirmedTransactions
      x-api-path-slug: unconfirmedtransactions-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
---