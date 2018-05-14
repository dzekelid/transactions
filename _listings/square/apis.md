---
name: Square
description: Starting with a free credit card reader for the iPhone, iPad, and Android
  devices, Square Reader allows anyone to accept credit cards anywhere, anytime, for
  a low transaction rate of 2.75 percent per swipe, with no hidden fees. Square Register
  serves as a full point-of-sale system for businesses to accept payments, manage
  items, and share menu and location information. Square Wallet, available in the
  US, is the most seamless way to pay, enabling individuals to pay at their favorite
  local businesses, discover new ones nearby, explore menu listings, and store receipts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Stack Network
- Payments
- Payment API
- Credit Cards
- Commerce
created: "2018-05-13"
modified: "2018-05-13"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/square/apis.md
specificationVersion: "0.14"
apis:
- name: Square Connect API Post V2 Locations Location Transactions
  description: |-
    Charges a card represented by a card nonce or a customer's card on file.

    Your request to this endpoint must include _either_:

    - A value for the `card_nonce` parameter (to charge a card nonce generated
    with the `SqPaymentForm`)
    - Values for the `customer_card_id` and `customer_id` parameters (to charge
    a customer's card on file)

    In order for an eCommerce payment to potentially qualify for
    [Square chargeback protection](https://squareup.com/help/article/5394), you
    _must_ provide values for the following parameters in your request:

    - `buyer_email_address`
    - At least one of `billing_address` or `shipping_address`

    When this response is returned, the amount of Square's processing fee might not yet be
    calculated. To obtain the processing fee, wait about ten seconds and call
    [RetrieveTransaction](#endpoint-retrievetransaction). See the `processing_fee_money`
    field of each [Tender included](#type-tender) in the transaction.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1/
  tags: Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/square/v2-locations-location-id-transactions-post.md
x-common:
- type: x-base
  url: https://connect.squareup.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/square
- type: x-developer
  url: https://connect.squareup.com/
- type: x-github
  url: https://github.com/square
- type: x-twitter
  url: https://twitter.com/Square
- type: x-website
  url: https://squareup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---