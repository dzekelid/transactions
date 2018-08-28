swagger: "2.0"
x-collection-name: Allied Irish Bank
x-complete: 1
info:
  title: Allied Irish Bank
  description: this-is-an-openapi-definition-for-the-standard-set-of-open-banking-httpopenbankingapis-io-apis-covering-the-allied-irish-bank-apis-
  termsOfService: https://www.openbanking.org.uk/open-licence/
  contact:
    name: API Evangelist
    url: https://apievangelist.com
    email: info@apievangelist.com
  version: 1.0.0
basePath: open-banking/v2.1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{AccountId}/transactions:
    get:
      summary: Get Account Transactions
      description: Get transactions related to an account
      operationId: GetAccountTransactions
      x-api-path-slug: accountsaccountidtransactions-get
      parameters:
      - in: path
        name: AccountId
        description: A unique identifier used to identify the account resource
      - in: header
        name: Authorization
        description: An Authorisation Token as per https://tools
      - in: query
        name: fromBookingDateTime
        description: The UTC ISO 8601 Date Time to filter transactions FROM NB Time
          component is optional - set to 00:00:00 for just Date
      - in: query
        name: toBookingDateTime
        description: The UTC ISO 8601 Date Time to filter transactions TO NB Time
          component is optional - set to 00:00:00 for just Date
      - in: header
        name: x-fapi-customer-ip-address
        description: The PSUs IP address if the PSU is currently logged in with the
          TPP
      - in: header
        name: x-fapi-customer-last-logged-time
        description: The time when the PSU last logged in with the TPP
      - in: header
        name: x-fapi-financial-id
        description: The unique id of the ASPSP to which the request is issued
      - in: header
        name: x-fapi-interaction-id
        description: An RFC4122 UID used as a correlation id
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Account
      - Transactions
  /transactions:
    get:
      summary: Get Transactions
      description: Get Transactions
      operationId: GetTransactions
      x-api-path-slug: transactions-get
      parameters:
      - in: header
        name: Authorization
        description: An Authorisation Token as per https://tools
      - in: query
        name: fromBookingDateTime
        description: The UTC ISO 8601 Date Time to filter transactions FROM NB Time
          component is optional - set to 00:00:00 for just Date
      - in: query
        name: toBookingDateTime
        description: The UTC ISO 8601 Date Time to filter transactions TO NB Time
          component is optional - set to 00:00:00 for just Date
      - in: header
        name: x-fapi-customer-ip-address
        description: The PSUs IP address if the PSU is currently logged in with the
          TPP
      - in: header
        name: x-fapi-customer-last-logged-time
        description: The time when the PSU last logged in with the TPP
      - in: header
        name: x-fapi-financial-id
        description: The unique id of the ASPSP to which the request is issued
      - in: header
        name: x-fapi-interaction-id
        description: An RFC4122 UID used as a correlation id
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Transactions
host: openapi.aibgb.co.uk