---
swagger: "2.0"
x-collection-name: PayJunction
x-complete: 0
info:
  title: PayJunction Delete Transactions Notes
  description: /transactions/{transactionid}/notes/{noteid}.
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
  /transactions:
    post:
      summary: Post Transactions
      description: /transactions/ (swiped cc).
      operationId: TransactionsPost6
      x-api-path-slug: transactions-post
      parameters:
      - in: formData
        name: action
      - in: formData
        name: amountBase
      - in: formData
        name: billingCompanyName
      - in: formData
        name: billingFirstName
      - in: formData
        name: billingLastName
      - in: formData
        name: cardTrack
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
  /transactions/:
    get:
      summary: Get Transactions
      description: 'Not Available At Time at Time of Publishing this collection: Get
        a list of transactions'
      operationId: TransactionsGet
      x-api-path-slug: transactions-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: offset
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
  /transactions/{transactionId}:
    get:
      summary: Get Transactions
      description: /transactions/{transactionid}.
      operationId: TransactionsByTransactionIdGet
      x-api-path-slug: transactionstransactionid-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
    put:
      summary: Put Transactions
      description: Update an unsettled transaction
      operationId: TransactionsByTransactionIdPut
      x-api-path-slug: transactionstransactionid-put
      parameters:
      - in: formData
        name: amountBase
      - in: formData
        name: amountReject
      - in: formData
        name: amountShipping
      - in: formData
        name: amountTax
      - in: formData
        name: amountTip
      - in: header
        name: Content-Type
      - in: formData
        name: status
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
  /transactions/{transactionId}/notes:
    get:
      summary: Get Transactions Notes
      description: Get a list of notes for a transaction
      operationId: TransactionsNotesByTransactionIdGet
      x-api-path-slug: transactionstransactionidnotes-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: offset
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
    post:
      summary: Post Transactions Notes
      description: /transactions/{transactionid}/notes/.
      operationId: TransactionsNotesByTransactionIdPost
      x-api-path-slug: transactionstransactionidnotes-post
      parameters:
      - in: formData
        name: note
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
  /transactions/{transactionId}/notes/{noteId}:
    get:
      summary: Get Transactions Notes
      description: /transactions/{transactionid}/notes/{noteid}.
      operationId: TransactionsNotesByTransactionIdAndNoteIdGet
      x-api-path-slug: transactionstransactionidnotesnoteid-get
      parameters:
      - in: path
        name: noteId
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
    put:
      summary: Put Transactions Notes
      description: /transactions/{transactionid}/notes/{noteid}.
      operationId: TransactionsNotesByTransactionIdAndNoteIdPut
      x-api-path-slug: transactionstransactionidnotesnoteid-put
      parameters:
      - in: formData
        name: note
      - in: path
        name: noteId
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
    delete:
      summary: Delete Transactions Notes
      description: /transactions/{transactionid}/notes/{noteid}.
      operationId: TransactionsNotesByTransactionIdAndNoteIdDelete
      x-api-path-slug: transactionstransactionidnotesnoteid-delete
      parameters:
      - in: path
        name: noteId
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
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