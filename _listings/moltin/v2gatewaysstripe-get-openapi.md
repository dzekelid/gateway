---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Get a gateway (stripe)
  description: This endpoint allows you to pay for an order using Braintree and a
    users credit card.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/gateways/stripe:
    get:
      summary: Get a gateway (stripe)
      description: This endpoint allows you to pay for an order using Braintree and
        a users credit card.
      operationId: V2GatewaysStripeGet
      x-api-path-slug: v2gatewaysstripe-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Gateway
      - (stripe)
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