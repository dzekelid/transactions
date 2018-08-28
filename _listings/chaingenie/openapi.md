swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 1
info:
  title: ChainGenie = DLT + Blockchain + Magic
  description: chaingenie-is-here-to-help-companies-enjoy-the-benefits-of-blockchain-technology-distributed-tamper-proof-record-keeping-consensus-between-distrusting-nodes-when-you-do-not-have-the-expensive-blockchain-resources-chaingenie-offers-a-hook-to-connect-your-existing-it-applications-to-popular-blockchain-networks-like-ethereum-bitcoin-blockchain-etc-with-great-ease---want-to-know-how-chaingenie-works-under-the-hood-download-our-flyer--httpchaingenie-comchaingenieflyer-pdfthe-following-is-only-teaser-documentation--for-full-information-email--a-hrefmailtomagicchaingenie-commagicchaingenie-comahrupdate-09262016-brullibanking-micro-services-addedliliapikey-is-required-for-invoking-any-micro-serviceliulemail-a-hrefmailtomagicchaingenie-commagicchaingenie-coma-for-your-sandbox-apikey-hrcoming-soon-brmagic-canvas--drag-and-drop-microservices-to-create-a-blockchain-application---iblockchain-made-easyihrwant-to-connect-with-me-on-linkedin-send-me-an-invite--a-hrefhttplinkedin-cominupriya-target-blankhttplinkedin-cominupriyaahrscript----function-i-s-o-g-r-a-m---------igoogleanalyticsobject--r-ir--ir--function--------------ir-q--ir-q---pusharguments---------ir-l--1--new-date-a--s-createelemento--m--s-getelementsbytagnameo0-a-async--1-a-src--g-m-parentnode-insertbeforea-m----window-document-script-httpswww-googleanalytics-comanalytics-js-ga----gacreate-ua825523031-auto----gasend-pageviewscript
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tradechain/GetItemsFilterSort:
    post:
      summary: Report / list of marketplace transactions
      description: "Use a combination of fields to get any type of report.  Ex. send
        specific seller name or id to get active for sale items by seller; send specific
        filehash to get status of a particular item/invoice; send itemPartNum to get
        a list of all products of that partnumber and send sort order as itemValue
        ascending to cheapest top list) . . . \r\n-\tfilterField (accepted items below,
        default \u2013 none)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemPartNum\r\no\tfileHash\r\no\tFileHash\r\n-\tsortField
        (accepted items below, default \u2013 itemValidUntil)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemValue\r\no\titemPartNum\r\no\titemValidUntil\r\n-\tsortOrder
        (default \u2013 desc)\r\no\tasc\r\no\tdesc\r\n-\tonSaleOnly (default \u2013
        true, only if not \u201CInactive\u201D)\r\no\ttrue\r\no\tfalse\r\n-\tmaxPrice
        (double; default - 0)"
      operationId: TradechainGetItemsFilterSortPost
      x-api-path-slug: tradechaingetitemsfiltersort-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: filterField
      - in: formData
        name: filterValue
      - in: formData
        name: maxPrice
      - in: formData
        name: onSaleOnly
      - in: formData
        name: sortField
      - in: formData
        name: sortOrder
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Report
      - ""
      - ""
      - List
      - Of
      - Marketplace
      - Transactions
  /ethledger/gettrans:
    get:
      summary: Document transactions
      description: Displays all transactions connected to this project / smart contract
      operationId: EthledgerGettransGet
      x-api-path-slug: ethledgergettrans-get
      parameters:
      - in: header
        name: ApiKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Transactions