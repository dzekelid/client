---
swagger: "2.0"
x-collection-name: Authentiq Connect
x-complete: 0
info:
  title: Authentiq Connect List clients
  description: Retrieve a list of clients.
  termsOfService: https://www.authentiq.com/tos/
  contact:
    name: Team Authentiq
    url: https://www.authentiq.com/
    email: hello@authentiq.com
  version: "1.0"
host: connect.authentiq.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /client:
    get:
      summary: List clients
      description: Retrieve a list of clients.
      operationId: client
      x-api-path-slug: client-get
      responses:
        200:
          description: OK
      tags:
      - Client
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