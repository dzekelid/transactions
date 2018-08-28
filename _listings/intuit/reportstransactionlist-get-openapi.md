---
swagger: "2.0"
x-collection-name: Intuit
x-complete: 0
info:
  title: QuickBooks Online V3 API Get Reports Transaction LIST
  description: "Report - Trial List \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/transaction%20list"
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/TransactionList:
    get:
      summary: Get Reports Transaction LIST
      description: "Report - Trial List \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/transaction%20list"
      operationId: getReportsTransactionlist
      x-api-path-slug: reportstransactionlist-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Transaction
      - LIST
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