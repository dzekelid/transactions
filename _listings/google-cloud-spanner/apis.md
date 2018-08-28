---
name: Google Cloud Spanner
x-slug: google-cloud-spanner
description: 'Cloud Spanner is the first and only relational database service that
  is both strongly consistent and horizontally scalable. With Cloud Spanner you enjoy
  all the traditional benefits of a relational database: ACID transactions, relational
  schemas (and schema changes without downtime), SQL queries, high performance, and
  high availability. But unlike any other relational database service, Cloud Spanner
  scales horizontally, to hundreds or thousands of servers, so it can handle the highest
  of transactional workloads. With automatic scaling, synchronous data replication,
  and node redundancy, Cloud Spanner delivers up to 99.999% (five 9s) of availability
  for your mission critical applications. In fact, Google&rsquo;s internal Spanner
  service has been handling millions of queries per second from many Google services
  for years.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Transactions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/google-cloud-spanner/apis.md
specificationVersion: "0.14"
apis:
- name: Cloud Spanner - Begin Transaction
  x-api-slug: v1sessionbegintransaction-post
  description: |-
    Begins a new transaction. This step can often be skipped:
    Read, ExecuteSql and
    Commit can begin a new transaction as a
    side-effect.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/google-cloud-spanner/v1sessionbegintransaction-post-openapi.md
- name: Cloud Spanner - Commit Transaction
  x-api-slug: v1sessioncommit-post
  description: |-
    Commits a transaction. The request includes the mutations to be
    applied to rows in the database.

    `Commit` might return an `ABORTED` error. This can occur at any time;
    commonly, the cause is conflicts with concurrent
    transactions. However, it can also happen for a variety of other
    reasons. If `Commit` returns `ABORTED`, the caller should re-attempt
    the transaction from the beginning, re-using the same session.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/google-cloud-spanner/v1sessioncommit-post-openapi.md
- name: Cloud Spanner - Rollback Transaction
  x-api-slug: v1sessionrollback-post
  description: |-
    Rolls back a transaction, releasing any locks it holds. It is a good
    idea to call this for any transaction that includes one or more
    Read or ExecuteSql requests and
    ultimately decides not to commit.

    `Rollback` returns `OK` if it successfully aborts the transaction, the
    transaction was already aborted, or the transaction is not
    found. `Rollback` never returns `ABORTED`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/google-cloud-spanner/v1sessionrollback-post-openapi.md
- name: Cloud Spanner - Rollback Transaction
  x-api-slug: v1sessionrollback-post
  description: |-
    Rolls back a transaction, releasing any locks it holds. It is a good
    idea to call this for any transaction that includes one or more
    Read or ExecuteSql requests and
    ultimately decides not to commit.

    `Rollback` returns `OK` if it successfully aborts the transaction, the
    transaction was already aborted, or the transaction is not
    found. `Rollback` never returns `ABORTED`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/google-cloud-spanner/v1sessionrollback-post-openapi.md
- name: Cloud Spanner - Commit Transaction
  x-api-slug: v1sessioncommit-post
  description: |-
    Commits a transaction. The request includes the mutations to be
    applied to rows in the database.

    `Commit` might return an `ABORTED` error. This can occur at any time;
    commonly, the cause is conflicts with concurrent
    transactions. However, it can also happen for a variety of other
    reasons. If `Commit` returns `ABORTED`, the caller should re-attempt
    the transaction from the beginning, re-using the same session.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/google-cloud-spanner/v1sessioncommit-post-openapi.md
- name: Cloud Spanner - Begin Transaction
  x-api-slug: v1sessionbegintransaction-post
  description: |-
    Begins a new transaction. This step can often be skipped:
    Read, ExecuteSql and
    Commit can begin a new transaction as a
    side-effect.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transactions/master/_listings/google-cloud-spanner/v1sessionbegintransaction-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.source.repositories.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.spanner.stack.network
- type: x-change-log
  url: https://cloud.google.com/spanner/docs/release-notes
- type: x-code
  url: https://cloud.google.com/spanner/docs/reference/libraries
- type: x-command-line-interfaces
  url: https://cloud.google.com/spanner/docs/gcloud-spanner
- type: x-concepts
  url: https://cloud.google.com/spanner/docs/concepts
- type: x-documentation
  url: https://cloud.google.com/spanner/docs/
- type: x-getting-started
  url: https://cloud.google.com/spanner/docs/quickstart-console
- type: x-guide
  url: https://cloud.google.com/spanner/docs/how-to
- type: x-pricing
  url: https://cloud.google.com/spanner/pricing
- type: x-rate-limits
  url: https://cloud.google.com/spanner/docs/limits
- type: x-schema
  url: https://cloud.google.com/spanner/docs/information-schema
- type: x-service-level-agreements
  url: https://cloud.google.com/spanner/sla
- type: x-support
  url: https://cloud.google.com/spanner/docs/support
- type: x-website
  url: https://cloud.google.com/spanner/
- type: x-white-papers
  url: https://cloud.google.com/spanner/docs/whitepapers
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---