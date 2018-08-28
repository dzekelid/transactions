---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve a transaction's Lead Source
  description: Retrieve a Lead Source of given transaction
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transactions:
    get:
      summary: Retrieve a list of transactions
      description: Retrieve a list of transactions
      operationId: transactions.get
      x-api-path-slug: transactions-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Transactions
  /transactions/{id}/lead-source:
    get:
      summary: Retrieve a transaction's Lead Source
      description: Retrieve a Lead Source of given transaction
      operationId: transactions.id.lead_source.get
      x-api-path-slug: transactionsidleadsource-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Transactions
      - Lead
      - Source
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