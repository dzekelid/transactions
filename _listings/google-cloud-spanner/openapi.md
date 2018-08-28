swagger: "2.0"
x-collection-name: Google Cloud Spanner
x-complete: 1
info:
  title: Cloud Spanner
  description: cloud-spanner-is-a-managed-missioncritical-globally-consistent-and-scalable-relational-database-service-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: spanner.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{session}:beginTransaction:
    post:
      summary: Begin Transaction
      description: |-
        Begins a new transaction. This step can often be skipped:
        Read, ExecuteSql and
        Commit can begin a new transaction as a
        side-effect.
      operationId: spanner.projects.instances.databases.sessions.beginTransaction
      x-api-path-slug: v1sessionbegintransaction-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /v1/{session}:commit:
    post:
      summary: Commit Transaction
      description: |-
        Commits a transaction. The request includes the mutations to be
        applied to rows in the database.

        `Commit` might return an `ABORTED` error. This can occur at any time;
        commonly, the cause is conflicts with concurrent
        transactions. However, it can also happen for a variety of other
        reasons. If `Commit` returns `ABORTED`, the caller should re-attempt
        the transaction from the beginning, re-using the same session.
      operationId: spanner.projects.instances.databases.sessions.commit
      x-api-path-slug: v1sessioncommit-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /v1/{session}:rollback:
    post:
      summary: Rollback Transaction
      description: |-
        Rolls back a transaction, releasing any locks it holds. It is a good
        idea to call this for any transaction that includes one or more
        Read or ExecuteSql requests and
        ultimately decides not to commit.

        `Rollback` returns `OK` if it successfully aborts the transaction, the
        transaction was already aborted, or the transaction is not
        found. `Rollback` never returns `ABORTED`.
      operationId: spanner.projects.instances.databases.sessions.rollback
      x-api-path-slug: v1sessionrollback-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Transaction