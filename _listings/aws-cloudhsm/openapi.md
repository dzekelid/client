swagger: "2.0"
x-collection-name: AWS CloudHSM
x-complete: 1
info:
  title: AWS CloudHSM API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateLunaClient:
    get:
      summary: Create Luna Client
      description: Creates an HSM client.
      operationId: createLunaClient
      x-api-path-slug: actioncreatelunaclient-get
      parameters:
      - in: query
        name: Certificate
        description: The contents of a Base64-Encoded X
        type: string
      - in: query
        name: Label
        description: The label for the client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
  /?Action=DeleteLunaClient:
    get:
      summary: Delete Luna Client
      description: Deletes a client.
      operationId: deleteLunaClient
      x-api-path-slug: actiondeletelunaclient-get
      parameters:
      - in: query
        name: ClientArn
        description: The ARN of the client to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
  /?Action=DescribeLunaClient:
    get:
      summary: Describe Luna Client
      description: Retrieves information about an HSM client.
      operationId: describeLunaClient
      x-api-path-slug: actiondescribelunaclient-get
      parameters:
      - in: query
        name: CertificateFingerprint
        description: The certificate fingerprint
        type: string
      - in: query
        name: ClientArn
        description: The ARN of the client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
  /?Action=ListLunaClients:
    get:
      summary: List Luna Clients
      description: Lists all of the clients.
      operationId: listLunaClients
      x-api-path-slug: actionlistlunaclients-get
      parameters:
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to ListLunaClients
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
  /?Action=ModifyLunaClient:
    get:
      summary: Modify Luna Client
      description: Modifies the certificate used by the client.
      operationId: modifyLunaClient
      x-api-path-slug: actionmodifylunaclient-get
      parameters:
      - in: query
        name: Certificate
        description: The new certificate for the client
        type: string
      - in: query
        name: ClientArn
        description: The ARN of the client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients