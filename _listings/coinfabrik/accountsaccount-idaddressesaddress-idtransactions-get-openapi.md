---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 0
info:
  title: "CoinFabrik List address\u2019s transactions"
  description: list transactions that have been sent to a specific address. Regular
    bitcoin address can be used in place of address_id but the address has to be associated
    to the correct account.
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}/addresses/{address_id}/transactions:
    get:
      summary: "List address\u2019s transactions"
      description: list transactions that have been sent to a specific address. Regular
        bitcoin address can be used in place of address_id but the address has to
        be associated to the correct account.
      operationId: list-transactions-that-have-been-sent-to-a-specific-address-regular-bitcoin-address-can-be-used-in-p
      x-api-path-slug: accountsaccount-idaddressesaddress-idtransactions-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: address_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - "Address\u2019s"
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