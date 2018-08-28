---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Gets the rti eps transaction template
  description: Return the rti eps transaction data object template
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Employer/{EmployerId}/RtiTransaction/{RtiTransactionId}:
    get:
      summary: Get the RTI transaction
      description: Returns the specified RTI transaction
      operationId: GetRtiTransactionFromEmployer
      x-api-path-slug: employeremployeridrtitransactionrtitransactionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: RtiTransactionId
        description: The RTI transaction unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Transaction
  /Templates/rtieastransaction:
    get:
      summary: Gets the rti eas transaction template
      description: Return the rti eas transaction data object template
      operationId: GetRtiEasTransactionTemplate
      x-api-path-slug: templatesrtieastransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Eas
      - Transaction
      - Template
  /Templates/rtiepstransaction:
    get:
      summary: Gets the rti eps transaction template
      description: Return the rti eps transaction data object template
      operationId: GetRtiEpsTransactionTemplate
      x-api-path-slug: templatesrtiepstransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Eps
      - Transaction
      - Template
  /Templates/rtieyutransaction:
    get:
      summary: Gets the rti eyu transaction template
      description: Return the rti eyu transaction data object template
      operationId: GetRtiEyuTransactionTemplate
      x-api-path-slug: templatesrtieyutransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Eyu
      - Transaction
      - Template
  /Templates/rtifpstransaction:
    get:
      summary: Gets the rti fps transaction template
      description: Return the rti fps transaction data object template
      operationId: GetRtiFpsTransactionTemplate
      x-api-path-slug: templatesrtifpstransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Fps
      - Transaction
      - Template
  /Templates/rtinvrtransaction:
    get:
      summary: Gets the rti nvr transaction template
      description: Return the rti nvr transaction data object template
      operationId: GetRtiNvrTransactionTemplate
      x-api-path-slug: templatesrtinvrtransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Nvr
      - Transaction
      - Template
  /Templates/rtitransactionbase:
    get:
      summary: Gets the rti transaction base template
      description: Return the rti transaction base data object template
      operationId: GetRtiTransactionBaseTemplate
      x-api-path-slug: templatesrtitransactionbase-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Transaction
      - Base
      - Template
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---