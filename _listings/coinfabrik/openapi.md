swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 1
info:
  title: Coinbase API
  description: the-coinbase-v2-api
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
  /accounts/{account_id}/transactions:
    get:
      summary: List transactions
      description: "Lists account\u2019s transactions. See Transaction resource for
        more information."
      operationId: lists-accounts-transactions-see-transaction-resource-for-more-information
      x-api-path-slug: accountsaccount-idtransactions-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - Transactions
  /accounts/{account_id}/transactions/{transaction_id}:
    get:
      summary: Show a transaction
      description: Show an individual transaction for an account. See Transaction
        resource for more information.
      operationId: show-an-individual-transaction-for-an-account-see-transaction-resource-for-more-information
      x-api-path-slug: accountsaccount-idtransactionstransaction-id-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: transaction_id
        description: The transaction id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Transaction