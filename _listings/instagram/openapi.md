swagger: "2.0"
x-collection-name: Instagram
x-complete: 1
info:
  title: Instagram
  version: 1.0.0
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;instagram-user-id&#125;/authorized_adaccounts:
    get:
      summary: Instagram User Authorized Adaccounts
      description: Instagram User Authorized Adaccounts
      operationId: getInstagramUserAuthorizedAdaccounts
      x-api-path-slug: 123instagramuserid125authorized-adaccounts-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - User
      - Authorized
      - Adaccounts