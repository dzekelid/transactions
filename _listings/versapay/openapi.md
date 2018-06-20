---
swagger: "2.0"
x-collection-name: VersaPay
x-complete: 1
info:
  title: VersaPay API Reference
  description: -introductionthe-versapay-api-offers-operations-in-support-of-its-flagship-products-arc--accounts-receivable-platform-with-automated-invoicing-effective-collaboration-flexible-payments-and-cash-application-to-improve-efficiency-and-customer-relationships----importing--exporting-customers-invoices-and-payments----monitoring-file-based-importsbatches--payport--cloud-based-platform-to-electronically-push-and-pull-funds-across-the-eft--ach-network----moving-funds-using-transactions-and-preauthorized-debit-agreements----a-secure-hosted-checkout-for-accepting-payments-through-your-website-or-email-please-contact-us-at-supportversapay-com-for-support--setup-of-ar-invoicing-integration-hosted-checkout-andor-payment-acceptance--environmentsthe-demo-environment-is-a-useful-sandbox-for-integration-testing-where-transaction-settlements-are-simulated-using-test-account-numbers-and-test-dollar-amounts-httpsdemo-versapay-comonce-integration-testing-is-complete-via-the-demo-environment-start-sending-your-requests-to-the-production-url-to-start-moving-money-andor-integrating-with-versapay-httpssecure-versapay-com-rate-limitsthere-is-a-60-request-per-minute-api-limit--any-requests-above-this-limit-will-result-in-http-return-code-403-forbidden-rate-limit-exceeded--access-to-api-keysvisit-your-account-settings-in-demohttpsdemo-versapay-comaccount-or-productionhttpssecure-versapay-comaccount-to-setup-api-keys-needed-for-authentication-as-well-as-webhooks-to-receive-relevant-callbacks-from-versapay-transaction-processing--you-can-generatedisable-your-api-keys-as-often-as-necessary-for-security-reasons-if-you-do-not-have-an-account-please-contact-versapay-support-for-support--setup-of-ar-invoicing-integration-hosted-checkout-andor-payment-acceptance--authenticationapi-requests-are-authenticated-using-http-basic-access-authenticationhttpsen-wikipedia-orgwikibasic-access-authentication--simply-provide-the-tokenkey-values-as-the-user-and-password-parameters-using-curl-for-instancecurl-u-nvax---un0i----x-post-httpssecure-versapay-comapi----testing-transactions-eft-bank-account-numbersin-the-demo-environment-the-following-test-bank-accounts-can-be-setup-up-in-your-account-institutioninstitution-numberbranchaccount-numbertd00499960112-digitsrbc00316824112-digitsbmo00199520112-digitshsbc01610880112-digitswhen-versapay-prompts-you-to-verify-these-bank-accounts-enter-a-value-of-1-23-for-the-verification-amount-to-determine-the-outcome-of-a-transaction-funded-by-a-bank-account-set-the-amount-accordinglyamountresulting-statex-10nsfedx-11completed-but-nsfedx-30erroranything-elsecompleted-ach-bank-account-numbersplease-contact-supportversapay-com-for-support--setup-of-ach-acceptance-and-bank-account-numbers-that-can-be-used-for-testing--credit-card-numbersplease-contact-supportversapay-com-for-support--setup-of-credit-card-acceptance-and-card-brandsnumbers-that-can-be-used-for-testing--tools-postmantry-out-the-api-using-postman-apphttpswww-getpostman-com-a-powerful-rest-api-client--download-the-versapay-api-reference-as-a-postman-collection-by-clicking-on-the-button-belowrun-in-postmanhttpsrun-pstmn-iobutton-svghttpsapp-getpostman-comruncollection7e34e0700a2f8c3074c6after-downloading-the-collection-set-up-and-configure-the-environment-as-follows1--download-the-sample-environment-filehttpsdevelopers-versapay-comdemo-postman-environment-json-2--import-the-environment-file-in-postman---import-environmenthttpsdevelopers-versapay-comimagesimport-environment-png3--once-it-is-imported-edit-the-environment-to-add-api-token-and-keys-associated-to-your-test-account---edit-environmenthttpsdevelopers-versapay-comimagesedit-environment-png4--click-update-to-save-your-changes-5--before-placing-api-calls-make-sure-the-correct-environment-is-selected---select-environmenthttpsdevelopers-versapay-comimagesselect-environment-png
  contact:
    name: VersaPay Support
    url: https://www.versapay.com/support
    email: support@versapay.com
  version: 1.0.0
host: secure.versapay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/transactions:
    get:
      summary: View Transactions
      description: View transactions.
      operationId: viewAllTransactions
      x-api-path-slug: apitransactions-get
      parameters:
      - in: query
        name: page
        description: 50 items are displayed per page
      responses:
        200:
          description: OK
      tags:
      - View
      - ""
      - Transactionss
    post:
      summary: Create Transactions
      description: Create transactions.
      operationId: createTransaction
      x-api-path-slug: apitransactions-post
      parameters:
      - in: body
        name: body
        description: Transaction to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ""
      - Transactionss
  /api/transactions/{token}:
    get:
      summary: View a Transaction
      description: View a transaction.
      operationId: viewTransaction
      x-api-path-slug: apitransactionstoken-get
      parameters:
      - in: path
        name: token
        description: The transaction identifier
      responses:
        200:
          description: OK
      tags:
      - View
      - Transactions
  /api/transactions/{token}/approve:
    post:
      summary: Approve a Transaction
      description: |-
        Approve a `new` or `wait_for_request_approval` transaction.<br>
        An API key with administrative access is required to approve a transaction.
      operationId: approveTransaction
      x-api-path-slug: apitransactionstokenapprove-post
      parameters:
      - in: body
        name: fund_token
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: token
        description: The transaction identifier
      responses:
        200:
          description: OK
      tags:
      - Approve
      - Transactions
  /api/transactions/{token}/cancel:
    post:
      summary: Cancel a Transaction
      description: |-
        Cancel a `new`, `wait_for_request_approval` or `wait_for_bank_account_verification` transaction you created. Transactions cannot be cancelled after they have been sent to the bank and are `in_progress`.<br>
        An API key with administrative access is required to approve a transaction.
      operationId: cancelTransaction
      x-api-path-slug: apitransactionstokencancel-post
      parameters:
      - in: path
        name: token
        description: The transaction identifier
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Transactions
---