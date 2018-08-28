---
name: Blockchain Info
x-slug: blockchain-info
description: With the largest bitcoin wallet platform in the world, Blockchain???s
  software has powered over 100M transactions and empowered users in 130 countries
  across the globe to transact quickly and without costly intermediaries. We also
  offers tools for develo...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28138-blockchain-info.jpg
x-kinRank: "8"
x-alexaRank: "842"
tags: Transactions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/blockchain-info/apis.md
specificationVersion: "0.14"
apis:
- name: Blockchain Info Raw Transaction
  x-api-slug: blockchain-info
  description: Returns a raw trasaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28138-blockchain-info.jpg
  humanURL: https://blockchain.info
  baseURL: https://blockchain.info///rawtx/{tx_hash}
  tags: Blockchain,Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/blockchain-info/rawtxtx-hash-get-openapi.md
- name: Blockchain Info Unconfirmed Transactions
  x-api-slug: blockchain-info
  description: Returns unconfirmed transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28138-blockchain-info.jpg
  humanURL: https://blockchain.info
  baseURL: https://blockchain.info///unconfirmed-transactions
  tags: Blockchain,Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/blockchain-info/unconfirmedtransactions-get-openapi.md
- name: Blockchain Info
  x-api-slug: blockchain-info
  description: With the largest bitcoin wallet platform in the world, Blockchain???s
    software has powered over 100M transactions and empowered users in 130 countries
    across the globe to transact quickly and without costly intermediaries. We also
    offers tools for develo...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28138-blockchain-info.jpg
  humanURL: https://blockchain.info
  baseURL: https://blockchain.info/
  tags: Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/blockchain-info/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/blockchain-info
- type: x-documentation
  url: https://blockchain.info/api
- type: x-twitter
  url: https://twitter.com/blockchain
- type: x-website
  url: https://blockchain.info
- type: x-websockets
  url: https://blockchain.info/api/api_websocket
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---