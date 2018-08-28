---
swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Accounting
  description: -introductionthe-xero-accounting-api-is-a-restful-web-service-and-uses-the-oauth-v1-0a-protocol-to-authenticate-3rd-party-applications--the-accounting-api-exposes-accounting-and-related-functions-of-the-main-xero-application-and-can-be-used-for-a-variety-of-purposes-such-as-creating-transactions-like-invoices-and-credit-notes-right-through-to-extracting-accounting-data-via-our-reports-endpoint-
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
    put:
      summary: Put Linkedtransactions
      description: Put linkedtransactions.
      operationId: putLinkedtransactions
      x-api-path-slug: linkedtransactions-put
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
    x-related-model:
      summary: X-related-model Linkedtransactions
      description: X-related-model linkedtransactions.
      operationId: x-related-modelLinkedtransactions
      x-api-path-slug: linkedtransactions-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - LinkedTransactions
  /LinkedTransactions/{LinkedTransactionID}:
    delete:
      summary: Delete Linkedtransactions Linkedtransaction
      description: Delete linkedtransactions linkedtransaction.
      operationId: deleteLinkedtransactionsLinkedtransaction
      x-api-path-slug: linkedtransactionslinkedtransactionid-delete
      parameters:
      - in: path
        name: LinkedTransactionID
      responses:
        200:
          description: OK
      tags:
      - LinkedTransactions
      - LinkedTransactionID
    get:
      summary: Get Linkedtransactions Linkedtransaction
      description: Get linkedtransactions linkedtransaction.
      operationId: getLinkedtransactionsLinkedtransaction
      x-api-path-slug: linkedtransactionslinkedtransactionid-get
      parameters:
      - in: path
        name: LinkedTransactionID
      responses:
        200:
          description: OK
      tags:
      - LinkedTransactions
      - LinkedTransactionID
    post:
      summary: Post Linkedtransactions Linkedtransaction
      description: Post linkedtransactions linkedtransaction.
      operationId: postLinkedtransactionsLinkedtransaction
      x-api-path-slug: linkedtransactionslinkedtransactionid-post
      parameters:
      - in: path
        name: LinkedTransactionID
      - in: body
        name: LinkedTransactions
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - LinkedTransactions
      - LinkedTransactionID
    x-related-model:
      summary: X-related-model Linkedtransactions Linkedtransaction
      description: X-related-model linkedtransactions linkedtransaction.
      operationId: x-related-modelLinkedtransactionsLinkedtransaction
      x-api-path-slug: linkedtransactionslinkedtransactionid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - LinkedTransactions
      - LinkedTransactionID
---