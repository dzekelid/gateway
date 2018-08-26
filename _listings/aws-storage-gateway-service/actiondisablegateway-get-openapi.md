---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Disable Gateway
  version: 1.0.0
  description: Disables a gateway when the gateway is no longer functioning.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ActivateGateway:
    get:
      summary: Activate Gateway
      description: Activates the gateway you previously deployed on your host.
      operationId: activateGateway
      x-api-path-slug: actionactivategateway-get
      parameters:
      - in: query
        name: ActivationKey
        description: Your gateway activation key
        type: string
      - in: query
        name: GatewayName
        description: The name you configured for your gateway
        type: string
      - in: query
        name: GatewayRegion
        description: A value that indicates the region where you want to store the
          snapshot backups
        type: string
      - in: query
        name: GatewayTimezone
        description: A value that indicates the time zone you want to set for the
          gateway
        type: string
      - in: query
        name: GatewayType
        description: A value that defines the type of gateway to activate
        type: string
      - in: query
        name: MediumChangerType
        description: The value that indicates the type of medium changer to use for
          gateway-VTL
        type: string
      - in: query
        name: TapeDriveType
        description: The value that indicates the type of tape drive to use for gateway-VTL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=DeleteGateway:
    get:
      summary: Delete Gateway
      description: Deletes a gateway.
      operationId: deleteGateway
      x-api-path-slug: actiondeletegateway-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=DescribeGatewayInformation:
    get:
      summary: Describe Gateway Information
      description: |-
        Returns metadata about a gateway such as its name, network interfaces, configured
                 time zone, and the state (whether the gateway is running or not).
      operationId: describeGatewayInformation
      x-api-path-slug: actiondescribegatewayinformation-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=DisableGateway:
    get:
      summary: Disable Gateway
      description: Disables a gateway when the gateway is no longer functioning.
      operationId: disableGateway
      x-api-path-slug: actiondisablegateway-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
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