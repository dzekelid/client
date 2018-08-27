---
swagger: "2.0"
x-collection-name: Google Adsense
x-complete: 0
info:
  title: Google Adsense API Delete URL Channel
  version: 1.0.0
  description: Delete a URL channel from the host AdSense account.
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
    post:
      summary: Create Ad Unit
      description: Insert the supplied ad unit into the specified publisher AdSense
        account.
      operationId: adsensehost.accounts.adunits.insert
      x-api-path-slug: accountsaccountidadclientsadclientidadunits-post
      parameters:
      - in: path
        name: accountId
        description: Account which will contain the ad unit
      - in: path
        name: adClientId
        description: Ad client into which to insert the ad unit
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
    put:
      summary: Update Ad Unit
      description: Update the supplied ad unit in the specified publisher AdSense
        account.
      operationId: adsensehost.accounts.adunits.update
      x-api-path-slug: accountsaccountidadclientsadclientidadunits-put
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client which contains the ad unit
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
  /accounts/{accountId}/adclients/{adClientId}/adunits/{adUnitId}:
    delete:
      summary: Delete Ad Unit
      description: Delete the specified ad unit from the specified publisher AdSense
        account.
      operationId: adsensehost.accounts.adunits.delete
      x-api-path-slug: accountsaccountidadclientsadclientidadunitsadunitid-delete
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad unit
      - in: path
        name: adClientId
        description: Ad client for which to get ad unit
      - in: path
        name: adUnitId
        description: Ad unit to delete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Units
    get:
      summary: Get Ad Unit
      description: Get the specified host ad unit in this AdSense account.
      operationId: adsensehost.accounts.adunits.get
      x-api-path-slug: accountsaccountidadclientsadclientidadunitsadunitid-get
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad unit
      - in: path
        name: adClientId
        description: Ad client for which to get ad unit
      - in: path
        name: adUnitId
        description: Ad unit to get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Units
  /accounts/{accountId}/adclients/{adClientId}/adunits/{adUnitId}/adcode:
    get:
      summary: Get Ad Unit Code
      description: Get ad code for the specified ad unit, attaching the specified
        host custom channels.
      operationId: adsensehost.accounts.adunits.getAdCode
      x-api-path-slug: accountsaccountidadclientsadclientidadunitsadunitidadcode-get
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client with contains the ad unit
      - in: path
        name: adUnitId
        description: Ad unit to get the code for
      - in: query
        name: hostCustomChannelId
        description: Host custom channel to attach to the ad code
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Units
  /adclients:
    get:
      summary: Get Ad Clients
      description: List all host ad clients in this AdSense account.
      operationId: adsensehost.adclients.list
      x-api-path-slug: adclients-get
      parameters:
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
  /adclients/{adClientId}:
    get:
      summary: Get Ad Client
      description: Get information about one of the ad clients in the Host AdSense
        account.
      operationId: adsensehost.adclients.get
      x-api-path-slug: adclientsadclientid-get
      parameters:
      - in: path
        name: adClientId
        description: Ad client to get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Clients
  /adclients/{adClientId}/customchannels:
    get:
      summary: Get Custom Channels
      description: List all host custom channels in this AdSense account.
      operationId: adsensehost.customchannels.list
      x-api-path-slug: adclientsadclientidcustomchannels-get
      parameters:
      - in: path
        name: adClientId
        description: Ad client for which to list custom channels
      - in: query
        name: maxResults
        description: The maximum number of custom channels to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through custom channels
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    patch:
      summary: Update Custom Channels
      description: Update a custom channel in the host AdSense account. This method
        supports patch semantics.
      operationId: adsensehost.customchannels.patch
      x-api-path-slug: adclientsadclientidcustomchannels-patch
      parameters:
      - in: path
        name: adClientId
        description: Ad client in which the custom channel will be updated
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: customChannelId
        description: Custom channel to get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    post:
      summary: Create Custom Channels
      description: Add a new custom channel to the host AdSense account.
      operationId: adsensehost.customchannels.insert
      x-api-path-slug: adclientsadclientidcustomchannels-post
      parameters:
      - in: path
        name: adClientId
        description: Ad client to which the new custom channel will be added
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    put:
      summary: Update Custom Channel
      description: Update a custom channel in the host AdSense account.
      operationId: adsensehost.customchannels.update
      x-api-path-slug: adclientsadclientidcustomchannels-put
      parameters:
      - in: path
        name: adClientId
        description: Ad client in which the custom channel will be updated
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /adclients/{adClientId}/customchannels/{customChannelId}:
    delete:
      summary: Delete Custom Channel
      description: Delete a specific custom channel from the host AdSense account.
      operationId: adsensehost.customchannels.delete
      x-api-path-slug: adclientsadclientidcustomchannelscustomchannelid-delete
      parameters:
      - in: path
        name: adClientId
        description: Ad client from which to delete the custom channel
      - in: path
        name: customChannelId
        description: Custom channel to delete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    get:
      summary: Get Custom Channel
      description: Get a specific custom channel from the host AdSense account.
      operationId: adsensehost.customchannels.get
      x-api-path-slug: adclientsadclientidcustomchannelscustomchannelid-get
      parameters:
      - in: path
        name: adClientId
        description: Ad client from which to get the custom channel
      - in: path
        name: customChannelId
        description: Custom channel to get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /adclients/{adClientId}/urlchannels:
    get:
      summary: Get URL Channels
      description: List all host URL channels in the host AdSense account.
      operationId: adsensehost.urlchannels.list
      x-api-path-slug: adclientsadclientidurlchannels-get
      parameters:
      - in: path
        name: adClientId
        description: Ad client for which to list URL channels
      - in: query
        name: maxResults
        description: The maximum number of URL channels to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through URL channels
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
    post:
      summary: Add URL Channel
      description: Add a new URL channel to the host AdSense account.
      operationId: adsensehost.urlchannels.insert
      x-api-path-slug: adclientsadclientidurlchannels-post
      parameters:
      - in: path
        name: adClientId
        description: Ad client to which the new URL channel will be added
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /adclients/{adClientId}/urlchannels/{urlChannelId}:
    delete:
      summary: Delete URL Channel
      description: Delete a URL channel from the host AdSense account.
      operationId: adsensehost.urlchannels.delete
      x-api-path-slug: adclientsadclientidurlchannelsurlchannelid-delete
      parameters:
      - in: path
        name: adClientId
        description: Ad client from which to delete the URL channel
      - in: path
        name: urlChannelId
        description: URL channel to delete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
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