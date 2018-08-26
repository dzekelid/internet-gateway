---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Detach Internet Gateway
  version: 1.0.0
  description: Detaches an Internet gateway from a VPC, disabling connectivity between
    the Internet and the VPC.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
  /?Action=DeleteEgressOnlyInternetGateway:
    get:
      summary: Delete Egress Only Internet Gateway
      description: Deletes an egress-only Internet gateway.
      operationId: deleteegressonlyinternetgateway
      x-api-path-slug: actiondeleteegressonlyinternetgateway-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InternetGatewayId
        description: The ID of the Internet gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Internet Gateway
  /?Action=DeleteInternetGateway:
    get:
      summary: Delete Internet Gateway
      description: Deletes the specified Internet gateway.
      operationId: deleteinternetgateway
      x-api-path-slug: actiondeleteinternetgateway-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: EgressOnlyInternetGatewayId.N
        description: One or more egress-only Internet gateway IDs
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Internet Gateway
  /?Action=DescribeEgressOnlyInternetGateways:
    get:
      summary: Describe Egress Only Internet Gateways
      description: Describes one or more of your egress-only Internet gateways.
      operationId: describeegressonlyinternetgateways
      x-api-path-slug: actiondescribeegressonlyinternetgateways-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: InternetGatewayId.N
        description: One or more Internet gateway IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Internet Gateway
  /?Action=DetachInternetGateway:
    get:
      summary: Detach Internet Gateway
      description: Detaches an Internet gateway from a VPC, disabling connectivity
        between the Internet and the VPC.
      operationId: detachinternetgateway
      x-api-path-slug: actiondetachinternetgateway-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: KeyName
        description: A unique name for the key pair
        type: string
      responses:
        200:
          description: OK
      tags:
      - Internet Gateway
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