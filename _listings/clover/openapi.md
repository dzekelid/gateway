---
swagger: "2.0"
x-collection-name: Clover
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/gateway:
    get:
      summary: Get a merchant's payment gateway configuration
      description: Get a merchant's payment gateway configuration.
      operationId: GetMerchantGateway
      x-api-path-slug: v3merchantsmidgateway-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Gateway
---