swagger: "2.0"
x-collection-name: Rebilly
x-complete: 1
info:
  title: Rebilly
  description: -introductionthe-rebilly-api-is-built-on-http---our-api-is-restful---it-has-predictableresource-urls---it-returns-http-response-codes-to-indicate-errors---it-alsoaccepts-and-returns-json-in-the-http-body---you-can-use-your-favoritehttprest-library-for-your-programming-language-to-use-rebillys-api-oryou-can-use-one-of-our-sdks-currently-available-in-phphttpsgithub-comrebillyrebillyphpand-chttpsgithub-comrebillyrebillydotnetclient--authenticationwhen-you-sign-up-for-an-account-you-are-given-your-first-api-key-you-can-generate-additional-api-keys-and-delete-api-keys-as-you-mayneed-to-rotate-your-keys-in-the-future--you-authenticate-to-therebilly-api-by-providing-your-secret-key-in-the-request-header-rebilly-offers-three-forms-of-authentication--private-key-json-web-tokens-andpublic-key--private-key-authenticates-each-request-by-searching-for-the-presenceof-an-http-header-rebapikey--jwt-authenticates-each-request-by-the-http-header-authorization--public-key-authenticates-by-the-http-header-rebauth-read-more-on-this-below-rebilly-also-offers-json-web-tokens-jwt-authentication-where-you-can-controlthe-specific-granular-permissions-and-expiration-for-that-jwt---we-call-our-resourcefor-generating-jwt-sessionstagsessions-rebilly-also-has-a-clientside-authentication-scheme-that-uses-anapiuser-and-hmacsha1-signature-only-for-the-tokens-resource-sothat-you-may-safely-create-tokens-from-the-clientside-without-compromisingyour-secret-keys-never-share-your-secret-keys--keep-them-guarded-and-secure-the-clientside-authentication-scheme-uses-one-http-header-named-rebauth--redocinject-securitydefinitions--php-sdkfor-all-php-sdk-examples-provided-in-this-spec-you-will-need-to-configure-client-you-may-do-it-like-thisphpclient--new-rebillyclient----apikey--yourapikeyhere----baseurl--httpsapi-rebilly-com
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