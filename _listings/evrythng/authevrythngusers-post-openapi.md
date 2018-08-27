---
swagger: "2.0"
x-collection-name: EVRYTHNG
x-complete: 0
info:
  title: EVRYTHNG /auth/evrythng/users (A)
  description: APP creates a new EVRYTHNG user in it (using email/password).
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /auth/evrythng/users:
    post:
      summary: /auth/evrythng/users (A)
      description: APP creates a new EVRYTHNG user in it (using email/password).
      operationId: AuthEvrythngUsersPost
      x-api-path-slug: authevrythngusers-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Evrythng
      - Users
  /auth/evrythng/users/{USER_ID}/validate:
    post:
      summary: /user/{id}/validate (A)
      description: APP validates a user (which can then login & out).
      operationId: AuthEvrythngUsersValidateByUSERIDPost
      x-api-path-slug: authevrythngusersuser-idvalidate-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Evrythng
      - Users
      - USER
      - ID
      - Validate
  /auth/evrythng/:
    post:
      summary: /auth/evrythng (A)
      description: APP logs in an existing (and activated) user (with email/password).
      operationId: AuthEvrythngPost
      x-api-path-slug: authevrythng-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Evrythng
  /auth/all/logout:
    post:
      summary: /auth/all/logout (U)
      description: USER logs himself out (which renders the user API Key invalid).
      operationId: AuthAllLogoutPost
      x-api-path-slug: authalllogout-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Auth
      - ""
      - Logout
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