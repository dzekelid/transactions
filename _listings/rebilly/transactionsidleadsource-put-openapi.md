---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Create a Lead Source for a transaction
  description: Create a Lead Source for a transaction
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
    delete:
      summary: Delete a Lead Source for a transaction
      description: Delete a Lead Source that belongs to a certain transaction
      operationId: transactions.id.lead_source.delete
      x-api-path-slug: transactionsidleadsource-delete
      responses:
        200:
          description: OK
      tags:
      - Lead
      - Sourcea
      - Transaction
    put:
      summary: Create a Lead Source for a transaction
      description: Create a Lead Source for a transaction
      operationId: transactions.id.lead_source.put
      x-api-path-slug: transactionsidleadsource-put
      parameters:
      - in: body
        name: body
        description: Lead Source resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Lead
      - Sourcea
      - Transaction
  /transactions/{id}:
    get:
      summary: Retrieve a Transaction
      description: Retrieve a Transaction with specified identifier string
      operationId: transactions.id.get
      x-api-path-slug: transactionsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Transaction
  /transactions/{id}/cancel:
    post:
      summary: Cancel a pending or suspended transaction
      description: Cancel a scheduled transaction. Once handled a transaction cannot
        be canceled
      operationId: transactions.id.cancel.post
      x-api-path-slug: transactionsidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Pending
      - Suspended
      - Transaction
  /transactions/{id}/gateway-logs:
    get:
      summary: Retrieve a Transaction Gateway Logs
      description: Retrieve Gateway communication Logs for Transaction with specified
        identifier string
      operationId: transactions.id.gateway_logs.get
      x-api-path-slug: transactionsidgatewaylogs-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Transaction
      - Gateway
      - Logs
  /transactions/{id}/matched-rules:
    get:
      summary: Get matched rules for the transaction
      description: Get matched rules for the transaction
      operationId: transactions.id.matched_rules.get
      x-api-path-slug: transactionsidmatchedrules-get
      responses:
        200:
          description: OK
      tags:
      - Matched
      - Rulesthe
      - Transaction
  /transactions/{id}/refund:
    post:
      summary: Refund a Transaction
      description: |-
        Refund a Transaction with specified identifier string.
        Note that the refund will be in the same currency as the original transaction.
      operationId: transactions.id.refund.post
      x-api-path-slug: transactionsidrefund-post
      parameters:
      - in: body
        name: body
        description: Transaction resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Refund
      - Transaction
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