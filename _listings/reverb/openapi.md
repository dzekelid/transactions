---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /priceguide/{id}/transactions:
    get:
      summary: Get Pricegue Transactions
      description: Get a list of paginated transactions for a price guide.
      operationId: getPricegueTransactions
      x-api-path-slug: priceguideidtransactions-get
      parameters:
      - in: query
        name: condition
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Priceguide
      - Id
      - Transactions
  /priceguide/{id}/transactions/summary:
    get:
      summary: Get Pricegue Transactions Summary
      description: Get a summary of transactions for a given price guide
      operationId: getPricegueTransactionsSummary
      x-api-path-slug: priceguideidtransactionssummary-get
      parameters:
      - in: query
        name: condition
      - in: path
        name: id
      - in: query
        name: number_of_months
      responses:
        200:
          description: OK
      tags:
      - Priceguide
      - Id
      - Transactions
      - Summary
---