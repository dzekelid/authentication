---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Add a single authorization
  version: 1.0.0
  description: .Add a single authorization
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/authorizations/{authId}:
    get:
      summary: Get a single authorization
      description: Get a single authorization.
      operationId: GetAuthorization
      x-api-path-slug: v3merchantsmidauthorizationsauthid-get
      parameters:
      - in: path
        name: authId
      - in: query
        name: expand
        description: 'Expandable fields: [cardTransaction, dccInfo, germanInfo, appTracking,
          taxRates, lineItemPayments, refunds, order, tender, employee, transactionInfo]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Authorizations
      - AuthId
    post:
      summary: Add a single authorization
      description: .Add a single authorization
      operationId: UpdateAuthorization
      x-api-path-slug: v3merchantsmidauthorizationsauthid-post
      parameters:
      - in: path
        name: authId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Authorizations
      - AuthId
    delete:
      summary: Delete a single authorization
      description: .Delete a single authorization
      operationId: DeleteAuthorization
      x-api-path-slug: v3merchantsmidauthorizationsauthid-delete
      parameters:
      - in: path
        name: authId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Authorizations
      - AuthId
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