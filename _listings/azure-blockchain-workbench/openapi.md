swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 1
info:
  title: Azure Blockchain Workbench REST API
  description: the-azure-blockchain-workbench-rest-api-is-a-workbench-extensibility-point-which-allows-developers-to-create-and-manage-blockchain-applications-manage-users-and-organizations-within-a-consortium-integrate-blockchain-applications-into-services-and-platforms-perform-transactions-on-a-blockchain-and-retrieve-transactional-and-contract-data-from-a-blockchain-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/ledgers/connections/{connectionId}/transactions:
    get:
      summary: Get Ledgers Connections Transactions
      description: Lists the transactions for a connected blockchain network.
      operationId: TransactionsGet
      x-api-path-slug: apiv1ledgersconnectionsconnectionidtransactions-get
      parameters:
      - in: path
        name: connectionId
        description: The id of the connection
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Ledgers
      - Connections
      - Transactions
  /api/v1/ledgers/connections/{connectionId}/transactions/{transactionId}:
    get:
      summary: Get Ledgers Connections Transactions Transactionid
      description: Gets the transaction matching a specific transaction ID.
      operationId: TransactionGet
      x-api-path-slug: apiv1ledgersconnectionsconnectionidtransactionstransactionid-get
      parameters:
      - in: path
        name: connectionId
        description: The connectionId of the transaction
      - in: path
        name: transactionId
        description: The id of the transaction
      responses:
        200:
          description: OK
      tags:
      - Ledgers
      - Connections
      - Transactions
      - Transactionid