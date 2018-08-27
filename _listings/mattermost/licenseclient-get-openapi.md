---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get client license
  description: |-
    Get a subset of the server license needed by the client.
    ##### Permissions
    No permission required but having the `manage_system` permission returns more information.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /config/client:
    get:
      summary: Get client configuration
      description: |-
        Get a subset of the server configuration needed by the client.
        ##### Permissions
        No permission required.
      operationId: get-a-subset-of-the-server-configuration-needed-by-the-client-permissionsno-permission-required
      x-api-path-slug: configclient-get
      parameters:
      - in: query
        name: format
        description: Must be `old`, other formats not implemented yet
      responses:
        200:
          description: OK
      tags:
      - Client
      - Configuration
  /license/client:
    get:
      summary: Get client license
      description: |-
        Get a subset of the server license needed by the client.
        ##### Permissions
        No permission required but having the `manage_system` permission returns more information.
      operationId: get-a-subset-of-the-server-license-needed-by-the-client-permissionsno-permission-required-but-having
      x-api-path-slug: licenseclient-get
      parameters:
      - in: query
        name: format
        description: Must be `old`, other formats not implemented yet
      responses:
        200:
          description: OK
      tags:
      - Client
      - License
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