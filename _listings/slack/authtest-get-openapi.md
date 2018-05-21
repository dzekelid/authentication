---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Test Auth
  description: Checks authentication & identity.
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /auth.revoke:
    get:
      summary: Revoke Auth
      description: Revokes a token.
      operationId: auth_revoke
      x-api-path-slug: authrevoke-get
      parameters:
      - in: query
        name: test
        description: Setting this parameter to `1` triggers a _testing mode_ where
          the specified token will not actually be revoked
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Authentication
  /auth.test:
    get:
      summary: Test Auth
      description: Checks authentication & identity.
      operationId: auth_test
      x-api-path-slug: authtest-get
      parameters:
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Authentication
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