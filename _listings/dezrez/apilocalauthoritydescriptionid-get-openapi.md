---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get an Local Authority Description by its Id
  version: 1.0.0
  description: Get an local authority description by its id.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/ExternalProvider:
    get:
      summary: Returns a URL that will start the process of authorisation with the
        external provider - normally using the OAuth1/2 protocol suite.
      description: Returns a url that will start the process of authorisation with
        the external provider - normally using the oauth1/2 protocol suite..
      operationId: ExternalProvider_GetAuthoriseAgencyUrlByexternalProviderId
      x-api-path-slug: apiexternalprovider-get
      parameters:
      - in: query
        name: externalProviderId
        description: The external provider identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - URL
      - That
      - Will
      - Start
      - Process
      - Of
      - Authorisation
      - External
      - Provider
      - '-'
      - Normally
      - Using
      - OAuth1
      - "2"
      - Protocol
      - Suite
  /api/localauthoritydescription/Save:
    post:
      summary: Save or update an Local Authority Description
      description: Save or update an local authority description.
      operationId: LocalAuthorityDescription_SaveDescriptionBylocalAuthorityDescriptionDataContract
      x-api-path-slug: apilocalauthoritydescriptionsave-post
      parameters:
      - in: body
        name: localAuthorityDescriptionDataContract
        description: The local authority description to save
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Update
      - Local
      - Authority
      - Description
  /api/LocalAuthorityDescription/{id}:
    get:
      summary: Get an Local Authority Description by its Id
      description: Get an local authority description by its id.
      operationId: LocalAuthorityDescription_GetByid
      x-api-path-slug: apilocalauthoritydescriptionid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Local
      - Authority
      - Description
      - By
      - Its
      - Id
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