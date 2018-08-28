---
swagger: "2.0"
x-collection-name: AWS Direct Connect
x-complete: 0
info:
  title: AWS Direct Connect API Describe Virtual Gateways
  version: 1.0.0
  description: Returns a list of virtual private gateways owned by the AWS account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeVirtualGateways:
    get:
      summary: Describe Virtual Gateways
      description: Returns a list of virtual private gateways owned by the AWS account.
      operationId: describeVirtualGateways
      x-api-path-slug: actiondescribevirtualgateways-get
      parameters:
      - in: query
        name: virtualGateways
        description: A list of virtual private gateways
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual Gateways
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