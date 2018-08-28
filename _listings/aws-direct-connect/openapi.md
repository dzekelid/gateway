swagger: "2.0"
x-collection-name: AWS Direct Connect
x-complete: 1
info:
  title: AWS Direct Connect API
  version: 1.0.0
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