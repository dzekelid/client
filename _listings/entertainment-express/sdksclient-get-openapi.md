---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Returns a zip file of client SDK.
  description: Generate and download SDK's for using the API.  Requires a subscription
    key for authorization and a valid client.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /SDKs/{Client}:
    get:
      summary: Returns a zip file of client SDK.
      description: Generate and download SDK's for using the API.  Requires a subscription
        key for authorization and a valid client.
      operationId: GetSDK
      x-api-path-slug: sdksclient-get
      parameters:
      - in: path
        name: Client
        description: Client SDK
      - in: query
        name: RedirectToFile
        description: Redirect to download the zipped SDK
      responses:
        200:
          description: OK
      tags:
      - SDKs
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