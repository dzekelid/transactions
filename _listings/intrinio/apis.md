---
name: Intrinio
x-slug: intrinio
description: Market for financial data APIs and analytics applications built with
  those data feeds. Affordable, easy to access financial data for developers and investors
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IntrinioLogo-Green-optimized.png
x-kinRank: "8"
x-alexaRank: "321628"
tags: Transactions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/intrinio/apis.md
specificationVersion: "0.14"
apis:
- name: Intrinio API Insider Transactions by Company
  x-api-slug: intrinio-api
  description: Returns a list of all insider transactions in a company.  Criteria
    for being an insider include being a director, officer, or 10%+ owner in the company.  Transactions
    are detailed for both non-derivative and derivative transactions by the insider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IntrinioLogo-Green-optimized.png
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com////companies/insider_transactions
  tags: Market Data,Insider Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/intrinio/companiesinsider-transactions-get-openapi.md
- name: Intrinio API Insider Transactions By Owner
  x-api-slug: intrinio-api
  description: Returns a list of all insider transactions by an owner in as many companies
    as the owner may be considered an insider.  Criteria for being an insider include
    being a director, officer, or 10%+ owner in the company.  Transactions are detailed
    for both non-derivative and derivative transactions by the insider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IntrinioLogo-Green-optimized.png
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com////owners/insider_transactions
  tags: Market Data,Owners,Insider Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/intrinio/ownersinsider-transactions-get-openapi.md
- name: Intrinio API
  x-api-slug: intrinio-api
  description: Market for financial data APIs and analytics applications built with
    those data feeds. Affordable, easy to access financial data for developers and
    investors
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IntrinioLogo-Green-optimized.png
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com//
  tags: Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/intrinio/openapi.md
x-common:
- type: x-applications-showcase
  url: https://intrinio.com/marketplace/apps
- type: x-authentication
  url: http://docs.intrinio.com/#authentication
- type: x-blog
  url: http://blog.intrinio.com/
- type: x-blog-rss
  url: http://blog.intrinio.com/feed/
- type: x-code
  url: http://docs.intrinio.com/#sdks
- type: x-crunchbase
  url: https://crunchbase.com/organization/tribunat
- type: x-developer
  url: https://intrinio.com/we-love-developers
- type: x-documentation
  url: https://intrinio.com/marketplace/data
- type: x-email
  url: cfarley@intrinio.com
- type: x-email
  url: admin@intrinio.com
- type: x-email
  url: support@intrinio.com
- type: x-login
  url: https://intrinio.com/login
- type: x-partners
  url: https://intrinio.com/partners
- type: x-press
  url: https://intrinio.com/press
- type: x-rate-limits
  url: http://docs.intrinio.com/#limits
- type: x-selfservice-registration
  url: https://intrinio.com/signup
- type: x-spreadsheets
  url: http://docs.intrinio.com/#spreadsheet-add-ins
- type: x-support
  url: https://intrinio.com/help
- type: x-tutorial
  url: https://intrinio.com/tutorial/web_api
- type: x-twitter
  url: https://twitter.com/intrinio
- type: x-website
  url: https://intrinio.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---