swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateUserPoolClient:
    get:
      summary: Create User Pool Client
      description: Creates the user pool client.
      operationId: createUserPoolClient
      x-api-path-slug: actioncreateuserpoolclient-get
      parameters:
      - in: query
        name: ClientName
        description: The client name for the user pool client you would like to create
        type: string
      - in: query
        name: ExplicitAuthFlows
        description: The explicit authentication flows
        type: string
      - in: query
        name: GenerateSecret
        description: Boolean to specify whether you want to generate a secret for
          the user pool client            being created
        type: string
      - in: query
        name: ReadAttributes
        description: The read attributes
        type: string
      - in: query
        name: RefreshTokenValidity
        description: The validity of the refresh token, in days
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to create a
          user pool            client
        type: string
      - in: query
        name: WriteAttributes
        description: The write attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pool Clients
  /?Action=DeleteUserPoolClient:
    get:
      summary: Delete User Pool Client
      description: Allows the developer to delete the user pool client.
      operationId: deleteUserPoolClient
      x-api-path-slug: actiondeleteuserpoolclient-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete the
          client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=DescribeUserPoolClient:
    get:
      summary: Describe User Pool Client
      description: |-
        Client method for returning the configuration information and metadata of the
                    specified user pool client.
      operationId: describeUserPoolClient
      x-api-path-slug: actiondescribeuserpoolclient-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pool Clients
  /?Action=ListUserPoolClients:
    get:
      summary: List User Pool Clients
      description: Lists the clients that have been created for the specified user
        pool.
      operationId: listUserPoolClients
      x-api-path-slug: actionlistuserpoolclients-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of results you want the request to return
          when listing the user            pool clients
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to list user
          pool            clients
        type: string
      responses:
        200:
          description: OK
      tags:
      - user Pool Clients
  /?Action=UpdateUserPoolClient:
    get:
      summary: Update User Pool Client
      description: |-
        Allows the developer to update the specified user pool client and password
                    policy.
      operationId: updateUserPoolClient
      x-api-path-slug: actionupdateuserpoolclient-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: ClientName
        description: The client name from the update user pool client request
        type: string
      - in: query
        name: ExplicitAuthFlows
        description: Explicit authentication flows
        type: string
      - in: query
        name: ReadAttributes
        description: The read-only attributes of the user pool
        type: string
      - in: query
        name: RefreshTokenValidity
        description: The validity of the refresh token, in days
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to update the
          user pool            client
        type: string
      - in: query
        name: WriteAttributes
        description: The writeable attributes of the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pool Clients