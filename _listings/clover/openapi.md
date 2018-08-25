---
swagger: "2.0"
x-collection-name: Clover
x-complete: 1
info:
  title: ""
  version: 1.0.0
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
---