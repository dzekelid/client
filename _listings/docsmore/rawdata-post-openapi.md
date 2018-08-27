---
swagger: "2.0"
x-collection-name: Docsmore
x-complete: 0
info:
  title: Docsmore Returns raw data response as json FOR SINGLE CLIENT DOC
  description: This API call gets you underlying raw data of the document. All you
    need to do is supply Auth token and Document Key as part of the call
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /getclientdocs:
    post:
      summary: Get List of Client Documents By Document ID
      description: In order to export as PDf, you will need to have client document
        ID available for that specific document you are looking to download.
      operationId: GetclientdocsPost
      x-api-path-slug: getclientdocs-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Client
      - Documents
      - Document
      - ID
  /rawdata:
    post:
      summary: Returns raw data response as json FOR SINGLE CLIENT DOC
      description: This API call gets you underlying raw data of the document. All
        you need to do is supply Auth token and Document Key as part of the call
      operationId: RawdataPost
      x-api-path-slug: rawdata-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Raw
      - Data
      - Response
      - As
      - Json
      - FOR
      - SINGLE
      - CLIENT
      - DOC
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