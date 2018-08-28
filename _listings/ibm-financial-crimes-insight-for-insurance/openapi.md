swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 1
info:
  title: Financial Crimes Insight for Insurance public REST APIs
  description: these-are-the-financial-crimes-insight-for-insurance-public-rest-apis-used-by-clients-to-access-the-fcii-capabilities
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/transaction:
    put:
      summary: Insert transaction data into the database
      description: This method is used to insert transaction data into the database.  The
        XML schema is defined in the TRANSACTION.XSD file.
      operationId: putTransaction
      x-api-path-slug: ibmfciplatformfacttransaction-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Transaction
      - Data
      - Into
      - Database
  /ibm/fci/platform/fact/transaction/{id}:
    get:
      summary: Retrieve transaction data from the database, by its internal id
      description: This method is used to retrieve transaction data from the database
      operationId: getTransaction
      x-api-path-slug: ibmfciplatformfacttransactionid-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Transaction
      - Data
      - From
      - Database
      - ""
      - By
      - Its
      - Internal
      - Id