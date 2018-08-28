swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_transaction_hex:
    get:
      summary: get_transaction_hex
      description: get_transaction_hex
      operationId: get-transaction-hex
      x-api-path-slug: get-transaction-hex-get
      parameters:
      - in: query
        name: trx
        description: transaction hex
      responses:
        200:
          description: OK
      tags:
      - Get
      - Transaction
      - Hex
  /get_transaction:
    get:
      summary: get_transaction
      description: get_transaction
      operationId: get-transaction
      x-api-path-slug: get-transaction-get
      parameters:
      - in: query
        name: trxId
        description: transaction id
      responses:
        200:
          description: OK
      tags:
      - Get
      - Transaction
  /broadcast_transaction:
    get:
      summary: broadcast_transaction
      description: broadcast_transaction
      operationId: broadcast-transaction
      x-api-path-slug: broadcast-transaction-get
      parameters:
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - Broadcast
      - Transaction
  /broadcast_transaction_synchronous:
    get:
      summary: broadcast_transaction_synchronous
      description: broadcast_transaction_synchronous
      operationId: broadcast-transaction-synchronous
      x-api-path-slug: broadcast-transaction-synchronous-get
      parameters:
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - Broadcast
      - Transaction
      - Synchronous
  /broadcast_transaction_with_callback:
    get:
      summary: 'WARNING: can only be used in Steem node or in scripts broadcast_transaction_with_callback'
      description: broadcast_transaction_with_callback
      operationId: broadcast-transaction-with-callback
      x-api-path-slug: broadcast-transaction-with-callback-get
      parameters:
      - in: query
        name: confirmationCallback
        description: confirmationCallback function
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - 'WARNING:'
      - Can
      - Only
      - Be
      - Used
      - In
      - Steem
      - Node
      - In
      - Scripts
      - Broadcast
      - Transaction
      - Callback
  /set_pending_transaction_callback:
    get:
      summary: 'WARNING: can only be used in Steem node or in scripts set_pending_transaction_callback'
      description: set_pending_transaction_callback
      operationId: set-pending-transaction-callback-
      x-api-path-slug: set-pending-transaction-callback-get
      parameters:
      - in: query
        name: cb
        description: callback function
      responses:
        200:
          description: OK
      tags:
      - 'WARNING:'
      - Can
      - Only
      - Be
      - Used
      - In
      - Steem
      - Node
      - In
      - Scripts
      - Set
      - Pending
      - Transaction
      - Callback