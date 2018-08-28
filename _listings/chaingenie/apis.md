---
name: ChainGenie
x-slug: chaingenie
description: ChainGenie provides a plug and play platform that helps you connect your
  existing (or create new) applications to DLTs for lodging and workflow management
  using a simple easy to use user interface. ChainGenie is a platform to create blockchain
  apps that provide speed-to-market for companies looking to launch faster, rather
  than reinvent the wheel. Write your applications to run on popular Blockchain networks
  like Ethereum, Bitcoin Blockchain etc with great ease when you require to validate
  credentials or make your existing traditional applications use the power of DLT
  and blockchain overnight!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
x-kinRank: "7"
x-alexaRank: ""
tags: Transactions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/chaingenie/apis.md
specificationVersion: "0.14"
apis:
- name: ChainGenie = DLT + Blockchain + Magic - Report / list of marketplace transactions
  x-api-slug: tradechaingetitemsfiltersort-post
  description: "Use a combination of fields to get any type of report.  Ex. send specific
    seller name or id to get active for sale items by seller; send specific filehash
    to get status of a particular item/invoice; send itemPartNum to get a list of
    all products of that partnumber and send sort order as itemValue ascending to
    cheapest top list) . . . \r\n-\tfilterField (accepted items below, default \u2013
    none)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemPartNum\r\no\tfileHash\r\no\tFileHash\r\n-\tsortField
    (accepted items below, default \u2013 itemValidUntil)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemValue\r\no\titemPartNum\r\no\titemValidUntil\r\n-\tsortOrder
    (default \u2013 desc)\r\no\tasc\r\no\tdesc\r\n-\tonSaleOnly (default \u2013 true,
    only if not \u201CInactive\u201D)\r\no\ttrue\r\no\tfalse\r\n-\tmaxPrice (double;
    default - 0)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/chaingenie/tradechaingetitemsfiltersort-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/chaingenie/tradechaingetitemsfiltersort-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Document transactions
  x-api-slug: ethledgergettrans-get
  description: Displays all transactions connected to this project / smart contract
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/chaingenie/ethledgergettrans-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/chaingenie/ethledgergettrans-get-openapi.md
x-common:
- type: x-github
  url: https://github.com/ChainGenie
- type: x-website
  url: http://chaingenie.com
- type: x-api-gallery
  url: http://broadleaf.commerce.api.gallery.streamdata.io
- type: x-twitter
  url: https://twitter.com/ChainGenie
- type: x-website
  url: http://api.chaingenie.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---