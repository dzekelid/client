---
swagger: "2.0"
x-collection-name: AWS CloudHSM
x-complete: 0
info:
  title: AWS CloudHSM API Describe Luna Client
  version: 1.0.0
  description: Retrieves information about an HSM client.
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