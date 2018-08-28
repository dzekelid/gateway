---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve a Gateway Account
  description: Retrieve a Gateway Account with specified identifier string
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transactions/{id}/gateway-logs:
    get:
      summary: Retrieve a Transaction Gateway Logs
      description: Retrieve Gateway communication Logs for Transaction with specified
        identifier string
      operationId: transactions.id.gateway_logs.get
      x-api-path-slug: transactionsidgatewaylogs-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Transaction
      - Gateway
      - Logs
  /gateway-accounts:
    get:
      summary: Retrieve a list of gateway accounts
      description: Retrieve a list of gateway accounts
      operationId: retrieve-a-list-of-gateway-accounts
      x-api-path-slug: gatewayaccounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Gateway
      - Accounts
    post:
      summary: Create a Gateway Account
      description: Create a Gateway Account
      operationId: create-a-gateway-account
      x-api-path-slug: gatewayaccounts-post
      parameters:
      - in: body
        name: body
        description: Gateway Account resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gateway
      - Account
  /gateway-accounts/{id}:
    delete:
      summary: Delete a Gateway Account
      description: Delete a Gateway Account with predefined identifier string
      operationId: delete-a-gateway-account-with-predefined-identifier-string
      x-api-path-slug: gatewayaccountsid-delete
      responses:
        200:
          description: OK
      tags:
      - Gateway
      - Account
    get:
      summary: Retrieve a Gateway Account
      description: Retrieve a Gateway Account with specified identifier string
      operationId: retrieve-a-gateway-account-with-specified-identifier-string
      x-api-path-slug: gatewayaccountsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Gateway
      - Account
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