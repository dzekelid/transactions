swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/transactions:
    get:
      summary: Get Admin Transactions
      description: Get admin transactions.
      operationId: getApiV1AdminTransactions
      x-api-path-slug: apiv1admintransactions-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Transactions
  /api/v1/admin/transactions/{filter}:
    get:
      summary: Get Admin Transactions Filter
      description: Get admin transactions filter.
      operationId: getApiV1AdminTransactionsFilter
      x-api-path-slug: apiv1admintransactionsfilter-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: filter
      - in: query
        name: range.from
      - in: query
        name: range.to
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Transactions
      - Filter