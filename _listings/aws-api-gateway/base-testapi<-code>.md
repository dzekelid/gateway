---
swagger: "2.0"
info:
  title: AWS API Gateway API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  base:
    testapi</code>:
      summary: Basepathmapping Create
      description: Creates a new BasePathMapping resource
      operationId: basepathmappingCreate
      parameters:
      - in: header
        name: '&quot;basePath&quot;'
        type: string
      - in: header
        name: '&quot;restApiId&quot;'
        type: string
      - in: header
        name: '&quot;stage&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: query
        name: BlockDeviceMapping.N
        description: Information about one or more block device mappings
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: query
        name: Description
        description: A description for the new image
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: Name
        description: A name for the new image
        type: string
      - in: query
        name: NoReboot
        description: By default, Amazon EC2 attempts to shut down and reboot the instance
          before creating the image
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
definitions: []
x-collection-name: AWS API Gateway
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