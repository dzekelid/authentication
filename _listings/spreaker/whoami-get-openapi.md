---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 0
info:
  title: Spreaker API Get Authenticated User
  version: v1
  description: Retrieves information about the authenticated user.
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /whoami:
    get:
      summary: Get Authenticated User
      description: Retrieves information about the authenticated user.
      operationId: getWhoami
      x-api-path-slug: whoami-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Authenticated
      - User
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