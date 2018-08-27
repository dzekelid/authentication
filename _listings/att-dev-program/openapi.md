swagger: "2.0"
x-collection-name: AT&T Dev Program
x-complete: 1
info:
  title: AT&T Dev Program Merged API
  version: 1.0.0
host: api.att.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1/devicecapabilities/acr:authorization/capabilities:
    get:
      summary: Get Devicecapabilities Acr Authorization Capabilities
      description: /1/devicecapabilities/acr:authorization/capabilities
      operationId: 1devicecapabilitiesacrauthorizationcapabilities
      x-api-path-slug: 1devicecapabilitiesacrauthorizationcapabilities-get
      responses:
        200:
          description: OK
      tags:
      - Devicecapabilities
      - Acr:authorization
      - Capabilities