swagger: "2.0"
x-collection-name: Standard Chartered
x-complete: 1
info:
  title: Standard Chartered
  description: standard-chartered-plc-is-a-british-multinational-banking-and-financial-services-company-headquartered-in-london-england--it-operates-a-network-of-more-than-1200-branches-and-outlets-including-subsidiaries-associates-and-joint-ventures-across-more-than-70-countries-and-employs-around-87000-people--it-is-a-universal-bank-with-operations-in-consumer-corporate-and-institutional-banking-and-treasury-services--despite-its-uk-base-it-does-not-conduct-retail-banking-in-the-uk-and-around-90-of-its-profits-come-from-asia-africa-and-the-middle-east-
  termsOfService: https://www.sc.com/terms-and-conditions
  contact:
    name: Steve Spicer
    url: https://www.sc.com
    email: steven.spicer@sc.com
  version: 1.0.0
host: developer.sc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cib/service/s2b/api/v1/trade/{countryCode}/{customerId}/transactions:
    get:
      summary: Retrieve all trade finance transaction status for the current date
        (localised to tz)
      description: Retrieve all trade finance transaction status for the current date
        (localised to tz)
      operationId: getCibServiceS2bApiV1TradeCountrycodeCustomerTransactions
      x-api-path-slug: cibservices2bapiv1tradecountrycodecustomeridtransactions-get
      parameters:
      - in: path
        name: countryCode
        description: ISO Country Code
      - in: path
        name: customerId
        description: Customer Reference Id
      - in: query
        name: tz
        description: Timezone code (ISO-8601), e
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Banking
      - Cib
      - Service
      - S2b
      - Api
      - V1
      - Trade
      - Countrycode
      - Customer
      - Transactions
  /cib/service/s2b/api/v1/banks/scb/accounts/{accountId}/{viewId}/transaction-request-types:
    get:
      summary: Finds all support transaction types for a given account
      description: The ???GetTransactionTypes??? API upon successful user authentication
        and entitlement checks will return the supported transaction types for the
        specified account
      operationId: getCibServiceS2bApiV1BanksScbAccountsAccountViewTransactionRequestTypes
      x-api-path-slug: cibservices2bapiv1banksscbaccountsaccountidviewidtransactionrequesttypes-get
      parameters:
      - in: path
        name: accountId
      - in: header
        name: GroupId
      - in: header
        name: UserId
      - in: path
        name: viewId
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Banking
      - Cib
      - Service
      - S2b
      - Api
      - V1
      - Banks
      - Scb
      - Accounts
      - Account
      - View
      - Transaction
      - Request
      - Types
  /cib/service/s2b/api/v1/trade/{countryCode}/{customerId}/transaction/{transactionId}:
    get:
      summary: Retrieve trade finance transaction status for specific transaction
        reference Id
      description: Retrieve trade finance transaction status for specific transaction
        reference Id
      operationId: getCibServiceS2bApiV1TradeCountrycodeCustomerTransactionTransaction
      x-api-path-slug: cibservices2bapiv1tradecountrycodecustomeridtransactiontransactionid-get
      parameters:
      - in: path
        name: countryCode
        description: Country Code
      - in: path
        name: customerId
        description: Customer Reference Id
      - in: path
        name: transactionId
        description: Transaction Reference Id
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Banking
      - Cib
      - Service
      - S2b
      - Api
      - V1
      - Trade
      - Countrycode
      - Customer
      - Transaction
      - Transaction