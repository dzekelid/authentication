swagger: "2.0"
x-collection-name: Spreaker
x-complete: 1
info:
  title: Spreaker API
  version: v1
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