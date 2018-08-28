---
swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 0
info:
  title: Open Bank Project Get Account Transactions
  description: Get transactions related to an account
  termsOfService: https://www.openbanking.org.uk/terms
  contact:
    name: Service Desk
    email: ServiceDesk@openbanking.org.uk
  version: 1.0.0
basePath: /open-banking/v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{AccountId}/transactions:
    get:
      summary: Get Account Transactions
      description: Get transactions related to an account
      operationId: GetAccountTransactions
      x-api-path-slug: accountsaccountidtransactions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Transactions
  /accounts/{AccountId}/statements/{StatementId}/transactions:
    get:
      summary: Get Statement Transactions
      description: Get Statement Transactions related to an account
      operationId: GetAccountStatementTransactions
      x-api-path-slug: accountsaccountidstatementsstatementidtransactions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Statement
      - Transactions
  /transactions:
    get:
      summary: Get Transactions
      description: Get Transactions
      operationId: GetTransactions
      x-api-path-slug: transactions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
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