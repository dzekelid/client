---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
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
---