---
name: Xero
x-slug: xero
description: Xero is the QuickBooks alternative. Use Xero accounting software to manage
  invoicing, bank reconciliation, bookkeeping & more. Start a free trial today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
x-kinRank: "8"
x-alexaRank: "2158"
tags: Transactions
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/apis.md
specificationVersion: "0.14"
apis:
- name: Clarity Accounting Get Bank Transactions
  x-api-slug: clarity-accounting
  description: Get banktransactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions
  tags: BankTransactions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactions-get-openapi.md
- name: Clarity Accounting Post Bank Transactions
  x-api-slug: clarity-accounting
  description: Post banktransactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions
  tags: BankTransactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactions-post-openapi.md
- name: Clarity Accounting Put Bank Transactions
  x-api-slug: clarity-accounting
  description: Put banktransactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions
  tags: BankTransactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactions-put-openapi.md
- name: Clarity Accounting X-related-model Bank Transactions
  x-api-slug: clarity-accounting
  description: X-related-model banktransactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions
  tags: BankTransactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactions-xrelatedmodel-openapi.md
- name: Clarity Accounting Get Bank Transactions Banktransaction
  x-api-slug: clarity-accounting
  description: Get banktransactions banktransaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions/{BankTransactionID}
  tags: BankTransactions,BankTransactionID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactionsbanktransactionid-get-openapi.md
- name: Clarity Accounting Post Bank Transactions Banktransaction
  x-api-slug: clarity-accounting
  description: Post banktransactions banktransaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions/{BankTransactionID}
  tags: BankTransactions,BankTransactionID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactionsbanktransactionid-post-openapi.md
- name: Clarity Accounting X-related-model Bank Transactions Banktransaction
  x-api-slug: clarity-accounting
  description: X-related-model banktransactions banktransaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions/{BankTransactionID}
  tags: BankTransactions,BankTransactionID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactionsbanktransactionid-xrelatedmodel-openapi.md
- name: Clarity Accounting Get Bank Transactions Banktransaction Attachments
  x-api-slug: clarity-accounting
  description: Get banktransactions banktransaction attachments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions/{BankTransactionID}/Attachments
  tags: BankTransactions,BankTransactionID,Attachments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactionsbanktransactionidattachments-get-openapi.md
- name: Clarity Accounting Get Bank Transactions Banktransaction Attachments Filename
  x-api-slug: clarity-accounting
  description: Get banktransactions banktransaction attachments filename.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions/{BankTransactionID}/Attachments/{FileName}
  tags: BankTransactions,BankTransactionID,Attachments,FileName
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactionsbanktransactionidattachmentsfilename-get-openapi.md
- name: Clarity Accounting Post Bank Transactions Banktransaction Attachments Filename
  x-api-slug: clarity-accounting
  description: Post banktransactions banktransaction attachments filename.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//BankTransactions/{BankTransactionID}/Attachments/{FileName}
  tags: BankTransactions,BankTransactionID,Attachments,FileName
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/banktransactionsbanktransactionidattachmentsfilename-post-openapi.md
- name: Clarity Accounting Get Linkedtransactions
  x-api-slug: clarity-accounting
  description: Get linkedtransactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//LinkedTransactions
  tags: LinkedTransactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/linkedtransactions-get-openapi.md
- name: Clarity Accounting Post Linkedtransactions
  x-api-slug: clarity-accounting
  description: Post linkedtransactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//LinkedTransactions
  tags: LinkedTransactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/linkedtransactions-post-openapi.md
- name: Clarity Accounting Put Linkedtransactions
  x-api-slug: clarity-accounting
  description: Put linkedtransactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//LinkedTransactions
  tags: LinkedTransactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/linkedtransactions-put-openapi.md
- name: Clarity Accounting X-related-model Linkedtransactions
  x-api-slug: clarity-accounting
  description: X-related-model linkedtransactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//LinkedTransactions
  tags: LinkedTransactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/linkedtransactions-xrelatedmodel-openapi.md
- name: Clarity Accounting Delete Linkedtransactions Linkedtransaction
  x-api-slug: clarity-accounting
  description: Delete linkedtransactions linkedtransaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//LinkedTransactions/{LinkedTransactionID}
  tags: LinkedTransactions,LinkedTransactionID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/linkedtransactionslinkedtransactionid-delete-openapi.md
- name: Clarity Accounting Get Linkedtransactions Linkedtransaction
  x-api-slug: clarity-accounting
  description: Get linkedtransactions linkedtransaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//LinkedTransactions/{LinkedTransactionID}
  tags: LinkedTransactions,LinkedTransactionID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/linkedtransactionslinkedtransactionid-get-openapi.md
- name: Clarity Accounting Post Linkedtransactions Linkedtransaction
  x-api-slug: clarity-accounting
  description: Post linkedtransactions linkedtransaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//LinkedTransactions/{LinkedTransactionID}
  tags: LinkedTransactions,LinkedTransactionID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/linkedtransactionslinkedtransactionid-post-openapi.md
- name: Clarity Accounting X-related-model Linkedtransactions Linkedtransaction
  x-api-slug: clarity-accounting
  description: X-related-model linkedtransactions linkedtransaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0//LinkedTransactions/{LinkedTransactionID}
  tags: LinkedTransactions,LinkedTransactionID
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/linkedtransactionslinkedtransactionid-xrelatedmodel-openapi.md
- name: Clarity Accounting
  x-api-slug: clarity-accounting
  description: Xero is the QuickBooks alternative. Use Xero accounting software to
    manage invoicing, bank reconciliation, bookkeeping & more. Start a free trial
    today!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/279-xero.jpg
  humanURL: http://www.xero.com/
  baseURL: https://api.xero.com//api.xro/2.0
  tags: Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/xero/openapi.md
x-common:
- type: x-base
  url: https://api.xero.com
- type: x-blog
  url: http://blog.xero.com
- type: x-blog
  url: https://devblog.xero.com/
- type: x-blog-rss
  url: https://devblog.xero.com/feed
- type: x-blog-rss
  url: http://feeds.feedburner.com/xerolive
- type: x-crunchbase
  url: http://www.crunchbase.com/company/xero
- type: x-crunchbase
  url: https://crunchbase.com/organization/xero
- type: x-developer
  url: http://developer.xero.com/
- type: x-email
  url: support@xero.com
- type: x-email
  url: sales@xero.com
- type: x-email
  url: careers@xero.com
- type: x-email
  url: privacy@xero.com
- type: x-email
  url: phishing@xero.com
- type: x-email
  url: press@xero.com
- type: x-email
  url: AUpress@xero.com
- type: x-email
  url: UKpress@xero.com
- type: x-email
  url: USpress@xero.com
- type: x-github
  url: https://github.com/XeroAPI
- type: x-partners
  url: http://developer.xero.com/partner/
- type: x-pricing
  url: https://www.xero.com/us/pricing/
- type: x-twitter
  url: https://twitter.com/xero
- type: x-website
  url: http://www.xero.com/
- type: x-website
  url: http://xero.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---