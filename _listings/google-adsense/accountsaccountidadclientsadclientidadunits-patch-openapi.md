---
swagger: "2.0"
x-collection-name: Google Adsense
x-complete: 0
info:
  title: Google Adsense API Update Ad Units
  version: 1.0.0
  description: Update the supplied ad unit in the specified publisher AdSense account.
    This method supports patch semantics.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/adclients:
    get:
      summary: Get Ad Clients
      description: List all hosted ad clients in the specified hosted account.
      operationId: adsensehost.accounts.adclients.list
      x-api-path-slug: accountsaccountidadclients-get
      parameters:
      - in: path
        name: accountId
        description: Account for which to list ad clients
      - in: query
        name: maxResults
        description: The maximum number of ad clients to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through ad clients
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Clients
  /accounts/{accountId}/adclients/{adClientId}:
    get:
      summary: Get Ad Client
      description: Get information about one of the ad clients in the specified publisher's
        AdSense account.
      operationId: adsensehost.accounts.adclients.get
      x-api-path-slug: accountsaccountidadclientsadclientid-get
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client to get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Clients
  /accounts/{accountId}/adclients/{adClientId}/adunits:
    get:
      summary: Get Ad Units
      description: List all ad units in the specified publisher's AdSense account.
      operationId: adsensehost.accounts.adunits.list
      x-api-path-slug: accountsaccountidadclientsadclientidadunits-get
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client for which to list ad units
      - in: query
        name: includeInactive
        description: Whether to include inactive ad units
      - in: query
        name: maxResults
        description: The maximum number of ad units to include in the response, used
          for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through ad units
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Units
    patch:
      summary: Update Ad Units
      description: Update the supplied ad unit in the specified publisher AdSense
        account. This method supports patch semantics.
      operationId: adsensehost.accounts.adunits.patch
      x-api-path-slug: accountsaccountidadclientsadclientidadunits-patch
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client which contains the ad unit
      - in: query
        name: adUnitId
        description: Ad unit to get
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Units
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