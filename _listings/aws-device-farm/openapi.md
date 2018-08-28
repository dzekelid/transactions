swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListOfferingTransactions:
    get:
      summary: List Offering Transactions
      description: |-
        Returns a list of all historical purchases, renewals, and system renewal transactions for an
              AWS account.
      operationId: listOfferingTransactions
      x-api-path-slug: actionlistofferingtransactions-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offering Transactions