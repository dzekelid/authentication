---
swagger: "2.0"
x-collection-name: Storecove
x-complete: 0
info:
  title: Storecove Get ShopAccounts with authorization failures
  description: |-
    Get ShopAccounts with authorization failures.
    include::examples/shop_accounts/shop_accounts_auth_failures/tabs.adoc[]
  version: 2.0.1
host: api.storecove.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shop_accounts/auth_failures:
    get:
      summary: Get ShopAccounts with authorization failures
      description: |-
        Get ShopAccounts with authorization failures.
        include::examples/shop_accounts/shop_accounts_auth_failures/tabs.adoc[]
      operationId: shop_accounts_auth_failures
      x-api-path-slug: shop-accountsauth-failures-get
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Accounts
      - Auth
      - Failures
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