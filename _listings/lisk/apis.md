---
name: Lisk
x-slug: lisk
description: Lisk makes it easy for developers to build and deploy blockchain applications
  in JavaScript. Join the leading platform for world-changing dapps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
x-kinRank: "7"
x-alexaRank: "145661"
tags: Transactions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/lisk/apis.md
specificationVersion: "0.14"
apis:
- name: Lisk API Documentation - Requests transactions data
  x-api-slug: transactions-get
  description: Search for a specified transaction in the system.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/lisk/transactions-get-openapi.md
- name: Lisk API Documentation - Submits a signature object to sign multisignature
    transactions
  x-api-slug: signatures-post
  description: |-
    Submits signature to sign a multisignature transaction.
    Signature objects can be generated locally either by using Lisk Commander or with Lisk Elements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/lisk/signatures-post-openapi.md
- name: Lisk API Documentation - Requests unprocessed transactions data
  x-api-slug: nodetransactionsstate-get
  description: |-
    By specifying the state of the transactions, you get a list of unprocessed transactions matching this state.
    Search for specific transactions by providing the appropriate parameters.
    If you post a batch of transactions, they will appear in the unprocessed list after a small delay, depending on server load.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/lisk/nodetransactionsstate-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://linkedin.api.gallery.streamdata.io
- type: x-crunchbase
  url: https://crunchbase.com/organization/lisk
- type: x-email
  url: support@lisk.io
- type: x-email
  url: dataprotection@lisk.io
- type: x-email
  url: help@lisk.io
- type: x-email
  url: business@lisk.io
- type: x-email
  url: events@lisk.io
- type: x-twitter
  url: https://twitter.com/LiskHQ
- type: x-website
  url: https://lisk.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---