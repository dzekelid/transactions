---
name: VersaPay
x-slug: versapay
description: VersaPay handles elements of both credit and debit card merchant payment
  processing in Canada. In offering a host of merchant account services and credit
  card POS terminals it allows for an efficient merchant payment service in all aspects-
  in person, on the go, online, and at the office. Founded in 2005 by Michael Gokturk,
  VersaPay is a Canadian owned and operated national financial transaction services
  provider partnered with Chase Paymentech. Versapay also offers electronic funds
  transfer through a system called Versapay EMT.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
x-kinRank: "9"
x-alexaRank: "410909"
tags: Transactions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apis.md
specificationVersion: "0.14"
apis:
- name: VersaPay API Reference - View a Transaction
  x-api-slug: apitransactionstoken-get
  description: View a transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstoken-get-openapi.md
- name: VersaPay API Reference - Approve a Transaction
  x-api-slug: apitransactionstokenapprove-post
  description: |-
    Approve a `new` or `wait_for_request_approval` transaction.<br>
    An API key with administrative access is required to approve a transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstokenapprove-post-openapi.md
- name: VersaPay API Reference - Cancel a Transaction
  x-api-slug: apitransactionstokencancel-post
  description: |-
    Cancel a `new`, `wait_for_request_approval` or `wait_for_bank_account_verification` transaction you created. Transactions cannot be cancelled after they have been sent to the bank and are `in_progress`.<br>
    An API key with administrative access is required to approve a transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstokencancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstokencancel-post-openapi.md
- name: VersaPay API Reference - View Transactions
  x-api-slug: apitransactions-get
  description: View transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-get-openapi.md
- name: VersaPay API Reference - Create Transactions
  x-api-slug: apitransactions-post
  description: Create transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-post-openapi.md
- name: VersaPay API Reference - View Transactions
  x-api-slug: apitransactions-get
  description: View transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-get-openapi.md
- name: VersaPay API Reference - Create Transactions
  x-api-slug: apitransactions-post
  description: Create transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-post-openapi.md
- name: VersaPay API Reference - View Transactions
  x-api-slug: apitransactions-get
  description: View transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-get-openapi.md
- name: VersaPay API Reference - Create Transactions
  x-api-slug: apitransactions-post
  description: Create transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-post-openapi.md
- name: VersaPay API Reference - View a Transaction
  x-api-slug: apitransactionstoken-get
  description: View a transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstoken-get-openapi.md
- name: VersaPay API Reference - Approve a Transaction
  x-api-slug: apitransactionstokenapprove-post
  description: |-
    Approve a `new` or `wait_for_request_approval` transaction.<br>
    An API key with administrative access is required to approve a transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstokenapprove-post-openapi.md
- name: VersaPay API Reference - Cancel a Transaction
  x-api-slug: apitransactionstokencancel-post
  description: |-
    Cancel a `new`, `wait_for_request_approval` or `wait_for_bank_account_verification` transaction you created. Transactions cannot be cancelled after they have been sent to the bank and are `in_progress`.<br>
    An API key with administrative access is required to approve a transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstokencancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactionstokencancel-post-openapi.md
- name: VersaPay API Reference - Create Transactions
  x-api-slug: apitransactions-post
  description: Create transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-post-openapi.md
- name: VersaPay API Reference - View Transactions
  x-api-slug: apitransactions-get
  description: View transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/versapay/apitransactions-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://venmo.api.gallery.streamdata.io
- type: x-api-stack
  url: http://versapay.stack.network
- type: x-base
  url: https://secure.versapay.com/api/
- type: x-blog
  url: https://www.versapay.com/blog/
- type: x-blog-rss
  url: http://www.versapay.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/versapay
- type: x-crunchbase
  url: https://crunchbase.com/organization/versapay
- type: x-github
  url: https://github.com/versapay
- type: x-partners
  url: https://www.versapay.com/partners/
- type: x-support
  url: https://www.versapay.com/support/
- type: x-twitter
  url: https://twitter.com/VersaPay
- type: x-website
  url: http://developers.versapay.com/index.html
- type: x-website
  url: https://www.versapay.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---