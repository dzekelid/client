swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
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