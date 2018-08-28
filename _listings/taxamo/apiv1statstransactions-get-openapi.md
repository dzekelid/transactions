---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 0
info:
  title: Taxamo Transaction Stats
  description: Transaction stats.
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/transactions:
    get:
      summary: Browse Transactions
      description: Browse transactions.
      operationId: listTransactions
      x-api-path-slug: apiv1transactions-get
      parameters:
      - in: query
        name: currency_code
        description: Three letter ISO currency code
      - in: query
        name: filter_text
        description: Filtering expression
      - in: query
        name: format
        description: Output format - supports csv value for this operation
      - in: query
        name: has_note
        description: Return only transactions with a note field set
      - in: query
        name: invoice_number
        description: Transaction invoice number
      - in: query
        name: key_or_custom_id
        description: Taxamo provided transaction key or custom id
      - in: query
        name: limit
        description: Limit (no more than 1000, defaults to 100)
      - in: query
        name: offset
        description: Offset
      - in: query
        name: order_date_from
        description: Order date from in yyyy-MM-dd format
      - in: query
        name: order_date_to
        description: Order date to in yyyy-MM-dd format
      - in: query
        name: original_transaction_key
        description: Taxamo provided original transaction key
      - in: query
        name: sort_reverse
        description: If true, results are sorted in descending order
      - in: query
        name: statuses
        description: Comma separated list of of transaction statuses
      - in: query
        name: tax_country_code
        description: Two letter ISO tax country code
      - in: query
        name: tax_country_codes
        description: Comma separated list of two letter ISO tax country codes
      - in: query
        name: total_amount_greater_than
        description: Return only transactions with total amount greater than given
          number
      - in: query
        name: total_amount_less_than
        description: Return only transactions with total amount less than a given
          number
      responses:
        200:
          description: OK
      tags:
      - Browse
      - Transactions
    post:
      summary: Store Transaction
      description: Store transaction.
      operationId: createTransaction
      x-api-path-slug: apiv1transactions-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Store
      - Transaction
  /api/v1/stats/transactions:
    get:
      summary: Transaction Stats
      description: Transaction stats.
      operationId: getTransactionsStats
      x-api-path-slug: apiv1statstransactions-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      - in: query
        name: interval
        description: Interval
      responses:
        200:
          description: OK
      tags:
      - Transaction
      - Stats
  /api/v1/transactions/{key}:
    delete:
      summary: Delete Transaction
      description: Delete transaction.
      operationId: cancelTransaction
      x-api-path-slug: apiv1transactionskey-delete
      parameters:
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Transaction
    get:
      summary: Retrieve Transaction Data.
      description: Retrieve transaction data..
      operationId: getTransaction
      x-api-path-slug: apiv1transactionskey-get
      parameters:
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Transaction
      - Data
    put:
      summary: Update Transaction
      description: Update transaction.
      operationId: updateTransaction
      x-api-path-slug: apiv1transactionskey-put
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /api/v1/transactions/{key}/confirm:
    post:
      summary: Confirm Transaction
      description: Confirm transaction.
      operationId: confirmTransaction
      x-api-path-slug: apiv1transactionskeyconfirm-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Confirm
      - Transaction
  /api/v1/transactions/{key}/refunds:
    get:
      summary: Get Transaction Refunds
      description: Get transaction refunds.
      operationId: listRefunds
      x-api-path-slug: apiv1transactionskeyrefunds-get
      parameters:
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Transaction
      - Refunds
  /api/v1/transactions/{key}/unconfirm:
    post:
      summary: Un-confirm The Transaction
      description: Un-confirm the transaction.
      operationId: unconfirmTransaction
      x-api-path-slug: apiv1transactionskeyunconfirm-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Un-confirm
      - Transaction
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---