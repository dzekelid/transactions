---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Post Linkedtransactions
  description: Post linkedtransactions.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /BankTransactions:
    get:
      summary: Get Bank Transactions
      description: Get banktransactions.
      operationId: getBanktransactions
      x-api-path-slug: banktransactions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
    post:
      summary: Post Bank Transactions
      description: Post banktransactions.
      operationId: postBanktransactions
      x-api-path-slug: banktransactions-post
      parameters:
      - in: body
        name: BankTransactions
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
    put:
      summary: Put Bank Transactions
      description: Put banktransactions.
      operationId: putBanktransactions
      x-api-path-slug: banktransactions-put
      parameters:
      - in: body
        name: BankTransactions
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
    x-related-model:
      summary: X-related-model Bank Transactions
      description: X-related-model banktransactions.
      operationId: x-related-modelBanktransactions
      x-api-path-slug: banktransactions-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
  /BankTransactions/{BankTransactionID}:
    get:
      summary: Get Bank Transactions Banktransaction
      description: Get banktransactions banktransaction.
      operationId: getBanktransactionsBanktransaction
      x-api-path-slug: banktransactionsbanktransactionid-get
      parameters:
      - in: path
        name: BankTransactionID
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
    post:
      summary: Post Bank Transactions Banktransaction
      description: Post banktransactions banktransaction.
      operationId: postBanktransactionsBanktransaction
      x-api-path-slug: banktransactionsbanktransactionid-post
      parameters:
      - in: path
        name: BankTransactionID
      - in: body
        name: BankTransactions
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
    x-related-model:
      summary: X-related-model Bank Transactions Banktransaction
      description: X-related-model banktransactions banktransaction.
      operationId: x-related-modelBanktransactionsBanktransaction
      x-api-path-slug: banktransactionsbanktransactionid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
  /BankTransactions/{BankTransactionID}/Attachments:
    get:
      summary: Get Bank Transactions Banktransaction Attachments
      description: Get banktransactions banktransaction attachments.
      operationId: getBanktransactionsBanktransactionAttachments
      x-api-path-slug: banktransactionsbanktransactionidattachments-get
      parameters:
      - in: path
        name: BankTransactionID
        description: The Xero generated unique identifier for an bank transaction
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
      - Attachments
  /BankTransactions/{BankTransactionID}/Attachments/{FileName}:
    get:
      summary: Get Bank Transactions Banktransaction Attachments Filename
      description: Get banktransactions banktransaction attachments filename.
      operationId: getBanktransactionsBanktransactionAttachmentsFilename
      x-api-path-slug: banktransactionsbanktransactionidattachmentsfilename-get
      parameters:
      - in: path
        name: BankTransactionID
        description: The Xero generated unique identifier for an bank transaction
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
      - Attachments
      - FileName
    post:
      summary: Post Bank Transactions Banktransaction Attachments Filename
      description: Post banktransactions banktransaction attachments filename.
      operationId: postBanktransactionsBanktransactionAttachmentsFilename
      x-api-path-slug: banktransactionsbanktransactionidattachmentsfilename-post
      parameters:
      - in: path
        name: BankTransactionID
        description: The Xero generated unique identifier for an bank transaction
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
      - Attachments
      - FileName
  /LinkedTransactions:
    get:
      summary: Get Linkedtransactions
      description: Get linkedtransactions.
      operationId: getLinkedtransactions
      x-api-path-slug: linkedtransactions-get
      parameters:
      - in: query
        name: ContactID
        description: Filter by the ContactID
      - in: query
        name: No Name
      - in: query
        name: SourceTransactionID
        description: Filter by the SourceTransactionID
      - in: query
        name: Status
        description: Filter by the combination of ContactID and Status
      - in: query
        name: TargetTransactionID
        description: Filter by the TargetTransactionID
      responses:
        200:
          description: OK
      tags:
      - LinkedTransactions
    post:
      summary: Post Linkedtransactions
      description: Post linkedtransactions.
      operationId: postLinkedtransactions
      x-api-path-slug: linkedtransactions-post
      parameters:
      - in: body
        name: LinkedTransactions
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - LinkedTransactions
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