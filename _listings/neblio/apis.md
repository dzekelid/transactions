---
name: Neblio
x-slug: neblio
description: Neblio was born out of the need for simple and intuitive tools and solutions
  to drive the adoption of blockchain technology in the enterprise space. We are working
  on tools, services, and APIs that will simplify and revolutionize the way that businesses
  deploy next-generation applications on the Neblio Blockchain Platform.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
x-kinRank: "7"
x-alexaRank: "350300"
tags: Transactions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/apis.md
specificationVersion: "0.14"
apis:
- name: Neblio REST API Suite - Get transactions by block or address
  x-api-slug: instxs-get
  description: Returns all transactions by block or address
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/instxs-get-openapi.md
- name: Neblio REST API Suite - Get transactions by block or address
  x-api-slug: testnetinstxs-get
  description: Returns all transactions by block or address
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetinstxs-get-openapi.md
- name: Neblio REST API Suite - Broadcasts a signed raw transaction to the network
  x-api-slug: ntp1broadcast-post
  description: Broadcasts a signed raw transaction to the network. If successful returns
    the txid of the broadcast trasnaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1broadcast-post-openapi.md
- name: Neblio REST API Suite - Information On an NTP1 Transaction
  x-api-slug: ntp1transactioninfotxid-get
  description: Returns detailed information regarding an NTP1 transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1transactioninfotxid-get-openapi.md
- name: Neblio REST API Suite - Builds a transaction that issues a new NTP1 Token
  x-api-slug: ntp1issue-post
  description: Builds an unsigned raw transaction that issues a new NTP1 token on
    the Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1issue-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that sends an NTP1 Token
  x-api-slug: ntp1sendtoken-post
  description: Builds an unsigned raw transaction that sends an NTP1 token on the
    Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1sendtoken-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that burns an NTP1 Token
  x-api-slug: ntp1burntoken-post
  description: Builds an unsigned raw transaction that burns an NTP1 token on the
    Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1burntoken-post-openapi.md
- name: Neblio REST API Suite - Broadcasts a signed raw transaction to the network
    (not NTP1 specific)
  x-api-slug: instxsend-post
  description: Broadcasts a signed raw transaction to the network. If successful returns
    the txid of the broadcast trasnaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/instxsend-post-openapi.md
- name: Neblio REST API Suite - Returns transaction object
  x-api-slug: instxtxid-get
  description: Returns NEBL transaction object representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/instxtxid-get-openapi.md
- name: Neblio REST API Suite - Returns raw transaction hex
  x-api-slug: insrawtxtxid-get
  description: Returns raw transaction hex representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/insrawtxtxid-get-openapi.md
- name: Neblio REST API Suite - Broadcasts a signed raw transaction to the network
    (not NTP1 specific)
  x-api-slug: testnetinstxsend-post
  description: Broadcasts a signed raw transaction to the network. If successful returns
    the txid of the broadcast trasnaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetinstxsend-post-openapi.md
- name: Neblio REST API Suite - Returns transaction object
  x-api-slug: testnetinstxtxid-get
  description: Returns NEBL transaction object representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetinstxtxid-get-openapi.md
- name: Neblio REST API Suite - Returns raw transaction hex
  x-api-slug: testnetinsrawtxtxid-get
  description: Returns raw transaction hex representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetinsrawtxtxid-get-openapi.md
- name: Neblio REST API Suite - Broadcasts a signed raw transaction to the network
  x-api-slug: testnetntp1broadcast-post
  description: Broadcasts a signed raw transaction to the network. If successful returns
    the txid of the broadcast trasnaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1broadcast-post-openapi.md
- name: Neblio REST API Suite - Information On an NTP1 Transaction
  x-api-slug: testnetntp1transactioninfotxid-get
  description: Returns detailed information regarding an NTP1 transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1transactioninfotxid-get-openapi.md
- name: Neblio REST API Suite - Builds a transaction that issues a new NTP1 Token
  x-api-slug: testnetntp1issue-post
  description: Builds an unsigned raw transaction that issues a new NTP1 token on
    the Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1issue-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that sends an NTP1 Token
  x-api-slug: testnetntp1sendtoken-post
  description: Builds an unsigned raw transaction that sends an NTP1 token on the
    Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1sendtoken-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that burns an NTP1 Token
  x-api-slug: testnetntp1burntoken-post
  description: Builds an unsigned raw transaction that burns an NTP1 token on the
    Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1burntoken-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that burns an NTP1 Token
  x-api-slug: testnetntp1burntoken-post
  description: Builds an unsigned raw transaction that burns an NTP1 token on the
    Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1burntoken-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that sends an NTP1 Token
  x-api-slug: testnetntp1sendtoken-post
  description: Builds an unsigned raw transaction that sends an NTP1 token on the
    Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1sendtoken-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that issues a new NTP1 Token
  x-api-slug: testnetntp1issue-post
  description: Builds an unsigned raw transaction that issues a new NTP1 token on
    the Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1issue-post-openapi.md
- name: Neblio REST API Suite - Information On an NTP1 Transaction
  x-api-slug: testnetntp1transactioninfotxid-get
  description: Returns detailed information regarding an NTP1 transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1transactioninfotxid-get-openapi.md
- name: Neblio REST API Suite - Broadcasts a signed raw transaction to the network
  x-api-slug: testnetntp1broadcast-post
  description: Broadcasts a signed raw transaction to the network. If successful returns
    the txid of the broadcast trasnaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetntp1broadcast-post-openapi.md
- name: Neblio REST API Suite - Returns raw transaction hex
  x-api-slug: testnetinsrawtxtxid-get
  description: Returns raw transaction hex representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetinsrawtxtxid-get-openapi.md
- name: Neblio REST API Suite - Returns transaction object
  x-api-slug: testnetinstxtxid-get
  description: Returns NEBL transaction object representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetinstxtxid-get-openapi.md
- name: Neblio REST API Suite - Broadcasts a signed raw transaction to the network
    (not NTP1 specific)
  x-api-slug: testnetinstxsend-post
  description: Broadcasts a signed raw transaction to the network. If successful returns
    the txid of the broadcast trasnaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/testnetinstxsend-post-openapi.md
- name: Neblio REST API Suite - Returns raw transaction hex
  x-api-slug: insrawtxtxid-get
  description: Returns raw transaction hex representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/insrawtxtxid-get-openapi.md
- name: Neblio REST API Suite - Returns transaction object
  x-api-slug: instxtxid-get
  description: Returns NEBL transaction object representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/instxtxid-get-openapi.md
- name: Neblio REST API Suite - Broadcasts a signed raw transaction to the network
    (not NTP1 specific)
  x-api-slug: instxsend-post
  description: Broadcasts a signed raw transaction to the network. If successful returns
    the txid of the broadcast trasnaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/instxsend-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that burns an NTP1 Token
  x-api-slug: ntp1burntoken-post
  description: Builds an unsigned raw transaction that burns an NTP1 token on the
    Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1burntoken-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that sends an NTP1 Token
  x-api-slug: ntp1sendtoken-post
  description: Builds an unsigned raw transaction that sends an NTP1 token on the
    Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1sendtoken-post-openapi.md
- name: Neblio REST API Suite - Builds a transaction that issues a new NTP1 Token
  x-api-slug: ntp1issue-post
  description: Builds an unsigned raw transaction that issues a new NTP1 token on
    the Neblio blockchain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1issue-post-openapi.md
- name: Neblio REST API Suite - Information On an NTP1 Transaction
  x-api-slug: ntp1transactioninfotxid-get
  description: Returns detailed information regarding an NTP1 transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1transactioninfotxid-get-openapi.md
- name: Neblio REST API Suite - Broadcasts a signed raw transaction to the network
  x-api-slug: ntp1broadcast-post
  description: Broadcasts a signed raw transaction to the network. If successful returns
    the txid of the broadcast trasnaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/neblio/ntp1broadcast-post-openapi.md
x-common:
- type: x-blog-rss
  url: https://nebl.io/feed/
- type: x-documentation
  url: https://nebl.io/apidocs/index.html
- type: x-github
  url: http://github.com/NeblioTeam
- type: x-openapi
  url: https://raw.githubusercontent.com/NeblioTeam/neblio-api-swagger-docs/master/swagger.json
- type: x-api-gallery
  url: http://moltin.api.gallery.streamdata.io
- type: x-blog
  url: https://nebl.io/blog/
- type: x-twitter
  url: https://twitter.com/NeblioTeam
- type: x-website
  url: https://nebl.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---