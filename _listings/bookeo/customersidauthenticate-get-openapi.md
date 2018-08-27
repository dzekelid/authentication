---
swagger: "2.0"
x-collection-name: Bookeo
x-complete: 0
info:
  title: Bookeo Check a customer's password
  version: 1.0.0
  description: |-
    The customer's email address is the "username" used by Bookeo to authenticate customers.
     So to authenticate a customer your application would typically use GET /customers to search for customers with a given email address, and then GET /customers/{id}/authenticate to authenticate.
     Remember that there may be duplicate customer records with the same email address, ex. due to duplicate importing or manual record creation.
host: api.bookeo.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers/{id}/authenticate:
    get:
      summary: Check a customer's password
      description: |-
        The customer's email address is the "username" used by Bookeo to authenticate customers.
         So to authenticate a customer your application would typically use GET /customers to search for customers with a given email address, and then GET /customers/{id}/authenticate to authenticate.
         Remember that there may be duplicate customer records with the same email address, ex. due to duplicate importing or manual record creation.
      operationId: getCustomersAuthenticate
      x-api-path-slug: customersidauthenticate-get
      parameters:
      - in: path
        name: id
      - in: query
        name: password
        description: remember to use URL encoding
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Authenticate
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