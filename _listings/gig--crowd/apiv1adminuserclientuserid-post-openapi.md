---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Admin User Client Userid
  version: 1.0.0
  description: Post admin user client userid.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/user/client/{userId}:
    get:
      summary: Get Admin User Client Userid
      description: Get admin user client userid.
      operationId: getApiV1AdminUserClientUser
      x-api-path-slug: apiv1adminuserclientuserid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Client
      - Userid
    post:
      summary: Post Admin User Client Userid
      description: Post admin user client userid.
      operationId: postApiV1AdminUserClientUser
      x-api-path-slug: apiv1adminuserclientuserid-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Client
      - Userid
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