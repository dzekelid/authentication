---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/internal/lfs_authenticate:
    post:
      summary: Post Internal Lfs Authenticate
      description: Post internal lfs authenticate.
      operationId: postV3InternalLfsAuthenticate
      x-api-path-slug: v3internallfs-authenticate-post
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Lfs
      - Authenticate
---