---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 1
info:
  title: New Relic
  version: 1.0.0
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /key_transactions.{format}:
    get:
      summary: Get Key Transactions. Format
      description: "This API endpoint returns a paginated \nlist of the key transactions
        associated with your New Relic account.  The time range for summary data is
        the last 10 minutes.\n\nKey transactions can be filtered by their name or
        list of IDs.\n\nSee our documentation for a discussion of \nsummary data output."
      operationId: getKeyTransactions.Format
      x-api-path-slug: key-transactions-format-get
      parameters:
      - in: query
        name: filter[ids]
        description: Filter by policy IDs
        type: list
      - in: query
        name: filter[name]
        description: Filter by name
        type: string
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Key
      - Transactions.
      - Format
  /key_transactions/{id}.{format}:
    get:
      summary: Get Key Transactions  . Format
      description: "This endpoint returns a single key transaction, identified by
        ID. The time range for summary data is the last 10 minutes.\n\nSee our documentation
        for a discussion of \nsummary data output."
      operationId: getKeyTransactions.Format
      x-api-path-slug: key-transactionsid-format-get
      parameters:
      - in: path
        name: id
        description: Key transaction ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Key
      - Transactions
      - ""
      - .
      - Format
---