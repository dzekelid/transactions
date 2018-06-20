---
swagger: "2.0"
x-collection-name: Intrinio
x-complete: 1
info:
  title: Intrinio
  description: through-our-intrinio-data-marketplace-we-offer-a-wide-selection-of-financial-data-feeds-sourced-by-our-own-proprietary-processes-as-well-as-from-many-data-vendors--the-primary-application-of-the-intrinio-api-is-for-use-in-thirdparty-applications-and-integrations-or-for-endusers-utilizing-the-excel-addin-and-google-sheets-addon--the-intrinio-api-uses-https-verbs-and-a-restful-endpoint-structure-which-makes-it-easy-to-request-data-from-intrinio--basic-authentication-is-administered-over-https--responses-are-delivered-in-json-format-
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/insider_transactions:
    get:
      summary: Insider Transactions by Company
      description: Returns a list of all insider transactions in a company.  Criteria
        for being an insider include being a director, officer, or 10%+ owner in the
        company.  Transactions are detailed for both non-derivative and derivative
        transactions by the insider.
      operationId: insider-transactions-by-company
      x-api-path-slug: companiesinsider-transactions-get
      parameters:
      - in: query
        name: end_date
        description: 'the latest transaction date for which to return data: YYYY'
        type: string
      - in: query
        name: identifier
        description: 'the stock market ticker symbol associated with the companies
          common stock securities or the Central Index Key issued by the SEC, which
          is the unique identifier all company filings are issued under:'
        type: string
      - in: query
        name: page_number
        description: an integer greater than or equal to 1 for specifying the page
          number for the return values
        type: string
      - in: query
        name: page_size
        description: an integer greater than 1 for specifying the number of results
          on each page
        type: string
      - in: query
        name: start_date
        description: 'the earliest transaction date for which to return data: YYYY'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Insider Transactions
  /owners/insider_transactions:
    get:
      summary: Insider Transactions By Owner
      description: Returns a list of all insider transactions by an owner in as many
        companies as the owner may be considered an insider.  Criteria for being an
        insider include being a director, officer, or 10%+ owner in the company.  Transactions
        are detailed for both non-derivative and derivative transactions by the insider.
      operationId: insider-transactions-by-owner
      x-api-path-slug: ownersinsider-transactions-get
      parameters:
      - in: query
        name: identifier
        description: the Central Index Key issued by the SEC, which is the unique
          identifier all owner filings are issued under:CENTRAL INDEX KEY
        type: string
      - in: query
        name: page_number
        description: an integer greater than or equal to 1 for specifying the page
          number for the return values
        type: string
      - in: query
        name: page_size
        description: an integer greater than 1 for specifying the number of results
          on each page
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Owners
      - Insider Transactions
---