---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Admin Transactions
  version: 1.0.0
  description: Get admin transactions.
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