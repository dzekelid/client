---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 1
info:
  title: Entertainment Express
  description: your-gateway-to-building-incredible-movie-tv-and-game-content-discovery-experiences-
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
---