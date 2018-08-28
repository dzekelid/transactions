swagger: "2.0"
x-collection-name: NetLicensing
x-complete: 1
info:
  title: NetLicensing
  description: the-labs64-netlicensing-restful-api-gives-you-access-to-netlicensings-core-features--you-authenticate-to-the-netlicensing-api-by-providing-your-account-credentials-or-simply-use-our-demo-account--find-out-more-about-labs64-netlicensing-at-netlicensing-io-
  termsOfService: https://www.labs64.com/legal/terms-of-service/netlicensing
  version: 2.x
host: go.netlicensing.io
basePath: /core/v2/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transaction:
    get:
      summary: Transactions list
      description: Return a list of all transactions for the current vendor
      operationId: listTransactions
      x-api-path-slug: transaction-get
      responses:
        200:
          description: OK
      tags:
      - Transaction
    post:
      summary: Create transaction
      description: Creates a new transaction
      operationId: createTransaction
      x-api-path-slug: transaction-post
      parameters:
      - in: formData
        name: active
        description: always true for transactions
      - in: formData
        name: dateClosed
      - in: formData
        name: dateCreated
      - in: formData
        name: licenseeNumber
      - in: formData
        name: number
        description: Unique number (across all products of a vendor) that identifies
          the transaction
      - in: formData
        name: paymentMethod
      - in: formData
        name: source
        description: AUTO transaction for internal use only
      - in: formData
        name: status
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /transaction/{transactionNumber}:
    get:
      summary: Get transaction
      description: Return a transaction by transactionNumber
      operationId: getTransaction
      x-api-path-slug: transactiontransactionnumber-get
      parameters:
      - in: path
        name: transactionNumber
        description: Unique number (across all products of a vendor) that identifies
          the transaction
      responses:
        200:
          description: OK
      tags:
      - Transaction
      - TransactionNumber
    post:
      summary: Update transaction
      description: Sets the provided properties to a transaction. Return an updated
        transaction
      operationId: updateTransaction
      x-api-path-slug: transactiontransactionnumber-post
      parameters:
      - in: formData
        name: active
        description: always true for transactions
      - in: formData
        name: dateClosed
      - in: formData
        name: dateCreated
      - in: formData
        name: number
        description: Unique number (across all products of a vendor) that identifies
          the transaction
      - in: formData
        name: paymentMethod
      - in: formData
        name: source
        description: AUTO transaction for internal use only
      - in: formData
        name: status
      - in: path
        name: transactionNumber
        description: Unique number (across all products of a vendor) that identifies
          the transaction
      responses:
        200:
          description: OK
      tags:
      - Transaction
      - TransactionNumber