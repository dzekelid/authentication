---
swagger: "2.0"
x-collection-name: AWS Security Token Service
x-complete: 0
info:
  title: AWS Security Token Service API Decode Authorization Message
  version: 1.0.0
  description: |-
    Decodes additional information about the authorization status of a request from an
          encoded message returned in response to an AWS request.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DecodeAuthorizationMessage:
    get:
      summary: Decode Authorization Message
      description: |-
        Decodes additional information about the authorization status of a request from an
              encoded message returned in response to an AWS request.
      operationId: decodeAuthorizationMessage
      x-api-path-slug: actiondecodeauthorizationmessage-get
      parameters:
      - in: query
        name: EncodedMessage
        description: The encoded message that was returned with the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
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