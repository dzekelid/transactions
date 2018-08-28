swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/transactions/{transactionId}:
    get:
      summary: Get Transactions
      description: Get a transaction info
      operationId: get-a-transaction-info
      x-api-path-slug: v1transactionstransactionid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: header
        name: predix-zone-id
        description: tenantId
      - in: path
        name: transactionId
        description: transaction Id
      responses:
        200:
          description: OK
      tags:
      - Transactions