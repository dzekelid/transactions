---
swagger: "2.0"
info:
  title: Intrinio API Insider Transactions By Owner
  description: Returns a list of all insider transactions by an owner in as many companies
    as the owner may be considered an insider.  Criteria for being an insider include
    being a director, officer, or 10%+ owner in the company.  Transactions are detailed
    for both non-derivative and derivative transactions by the insider.
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /owners/insider_transactions:
    get:
      summary: Insider Transactions By Owner
      description: Returns a list of all insider transactions by an owner in as many
        companies as the owner may be considered an insider
      operationId: insider-transactions-by-owner
      parameters:
      - in: query
        name: identifier
        description: |2-
           the Central Index Key issued by the SEC, which is the unique identifier all owner filings are issued under:
          CENTRAL INDEX KEY
        type: string
      - in: query
        name: page_number
        description: ' an integer greater than or equal to 1 for specifying the page
          number for the return values'
        type: string
      - in: query
        name: page_size
        description: ' an integer greater than 1 for specifying the number of results
          on each page'
        type: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - owners
      - insider transactions
definitions: []
x-collection-name: Intrinio
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