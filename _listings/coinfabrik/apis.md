---
name: CoinFabrik
x-slug: coinfabrik
description: Our smart contract development and full stack blockchain development
  services are supported by more than 20 years of experience building and reviewing
  secure applications. CoinFabrik is a full stack blockchain development company.
  Our expertise range from extending cryptocurrency nodes like Bitcoin and Ethereum
  to providing high level APIs and UIs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
x-kinRank: "7"
x-alexaRank: "970321"
tags: Transactions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/coinfabrik/apis.md
specificationVersion: "0.14"
apis:
- name: "Coinbase API - List address\u2019s transactions"
  x-api-slug: accountsaccount-idaddressesaddress-idtransactions-get
  description: list transactions that have been sent to a specific address. Regular
    bitcoin address can be used in place of address_id but the address has to be associated
    to the correct account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/coinfabrik/accountsaccount-idaddressesaddress-idtransactions-get-openapi.md
- name: Coinbase API - List transactions
  x-api-slug: accountsaccount-idtransactions-get
  description: "Lists account\u2019s transactions. See Transaction resource for more
    information."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/coinfabrik/accountsaccount-idtransactions-get-openapi.md
- name: Coinbase API - Show a transaction
  x-api-slug: accountsaccount-idtransactionstransaction-id-get
  description: Show an individual transaction for an account. See Transaction resource
    for more information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/coinfabrik/accountsaccount-idtransactionstransaction-id-get-openapi.md
- name: Coinbase API - List transactions
  x-api-slug: accountsaccount-idtransactions-get
  description: "Lists account\u2019s transactions. See Transaction resource for more
    information."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/coinfabrik/accountsaccount-idtransactions-get-openapi.md
- name: Coinbase API - Show a transaction
  x-api-slug: accountsaccount-idtransactionstransaction-id-get
  description: Show an individual transaction for an account. See Transaction resource
    for more information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/coinfabrik/accountsaccount-idtransactionstransaction-id-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://blog.coinfabrik.com/feed/
- type: x-github
  url: https://github.com/CoinFabrik
- type: x-openapi
  url: https://raw.githubusercontent.com/CoinFabrik/coinbase-api-swagger/master/swagger.json
- type: x-api-gallery
  url: http://codefresh.api.gallery.streamdata.io
- type: x-api-stack
  url: http://coinfabrik.stack.network
- type: x-blog
  url: https://blog.coinfabrik.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/coinfabrik
- type: x-twitter
  url: https://twitter.com/coinfabrik
- type: x-website
  url: https://www.coinfabrik.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---