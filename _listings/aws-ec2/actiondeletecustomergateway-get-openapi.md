---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Delete Customer Gateway
  version: 1.0.0
  description: Deletes the specified customer gateway.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCustomerGateway:
    get:
      summary: Create Customer Gateway
      description: Provides information to AWS about your VPN customer gateway device.
      operationId: createcustomergateway
      x-api-path-slug: actioncreatecustomergateway-get
      parameters:
      - in: query
        name: CustomerGatewayId
        description: The ID of the customer gateway
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=CreateNatGateway:
    get:
      summary: Create Nat Gateway
      description: Creates a NAT gateway in the specified subnet.
      operationId: createnatgateway
      x-api-path-slug: actioncreatenatgateway-get
      parameters:
      - in: query
        name: NatGatewayId
        description: The ID of the NAT gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=DeleteNatGateway:
    get:
      summary: Delete Nat Gateway
      description: Deletes the specified NAT gateway.
      operationId: deletenatgateway
      x-api-path-slug: actiondeletenatgateway-get
      parameters:
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this request
        type: string
      - in: query
        name: NatGatewayId.N
        description: One or more NAT gateway IDs
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=AttachInternetGateway:
    get:
      summary: Attach Internet Gateway
      description: "Attaches an Internet gateway to a VPC, enabling connectivity between
        the Internet\n\t\t\t\tand the VPC."
      operationId: attachinternetgateway
      x-api-path-slug: actionattachinternetgateway-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the request
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC for which to create the egress-only Internet
          gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Internet Gateway
  /?Action=AttachVpnGateway:
    get:
      summary: Attach Vpn Gateway
      description: Attaches a virtual private gateway to a VPC.
      operationId: attachvpngateway
      x-api-path-slug: actionattachvpngateway-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone for the virtual private gateway
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: Type
        description: The type of VPN connection this virtual private gateway supports
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPN Gateway
  /?Action=CreateEgressOnlyInternetGateway:
    get:
      summary: Create Egress Only Internet Gateway
      description: '[IPv6 only] Creates an egress-only Internet gateway for your VPC.'
      operationId: createegressonlyinternetgateway
      x-api-path-slug: actioncreateegressonlyinternetgateway-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Internet Gateway
  /?Action=CreateInternetGateway:
    get:
      summary: Create Internet Gateway
      description: Creates an Internet gateway for use with a VPC.
      operationId: createinternetgateway
      x-api-path-slug: actioncreateinternetgateway-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: EgressOnlyInternetGatewayId
        description: The ID of the egress-only Internet gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Internet Gateway
  /?Action=CreateVpnGateway:
    get:
      summary: Create Vpn Gateway
      description: Creates a virtual private gateway.
      operationId: createvpngateway
      x-api-path-slug: actioncreatevpngateway-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: VpnGatewayId
        description: The ID of the virtual private gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPN Gateway
  /?Action=DeleteCustomerGateway:
    get:
      summary: Delete Customer Gateway
      description: Deletes the specified customer gateway.
      operationId: deletecustomergateway
      x-api-path-slug: actiondeletecustomergateway-get
      parameters:
      - in: query
        name: CustomerGatewayId.N
        description: One or more customer gateway IDs
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Customer Gateway
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