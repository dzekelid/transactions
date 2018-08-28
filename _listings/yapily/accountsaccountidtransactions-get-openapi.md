---
swagger: "2.0"
x-collection-name: Yapily
x-complete: 0
info:
  title: Yapily Get account transactions
  description: Get account transactions.
  version: 1.0.0
host: api.yapily.com:443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/transactions:
    get:
      summary: Get account transactions
      description: Get account transactions.
      operationId: getTransactionsUsingGET
      x-api-path-slug: accountsaccountidtransactions-get
      parameters:
      - in: path
        name: accountId
        description: accountId
      - in: header
        name: consent
        description: Consent Token
      responses:
        200:
          description: OK
      tags:
      - Account
      - Transactions
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