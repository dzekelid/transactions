---
swagger: "2.0"
x-collection-name: PayJunction
x-complete: 0
info:
  title: PayJunction Get Transactions
  description: 'Not Available At Time at Time of Publishing this collection: Get a
    list of transactions'
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transactions:
    post:
      summary: Post Transactions
      description: /transactions/ (swiped cc).
      operationId: TransactionsPost6
      x-api-path-slug: transactions-post
      parameters:
      - in: formData
        name: action
      - in: formData
        name: amountBase
      - in: formData
        name: billingCompanyName
      - in: formData
        name: billingFirstName
      - in: formData
        name: billingLastName
      - in: formData
        name: cardTrack
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
  /transactions/:
    get:
      summary: Get Transactions
      description: 'Not Available At Time at Time of Publishing this collection: Get
        a list of transactions'
      operationId: TransactionsGet
      x-api-path-slug: transactions-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: offset
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
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