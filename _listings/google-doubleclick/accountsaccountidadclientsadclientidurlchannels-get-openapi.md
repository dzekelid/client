---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get URL Channels
  version: 1.0.0
  description: List all URL channels in the specified ad client for this Ad Exchange
    account.
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
      description: List all ad clients in this Ad Exchange account.
      operationId: adexchangeseller.accounts.adclients.list
      x-api-path-slug: accountsaccountidadclients-get
      parameters:
      - in: path
        name: accountId
        description: Account to which the ad client belongs
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
  /accounts/{accountId}/adclients/{adClientId}/customchannels:
    get:
      summary: Get Custom Channels
      description: List all custom channels in the specified ad client for this Ad
        Exchange account.
      operationId: adexchangeseller.accounts.customchannels.list
      x-api-path-slug: accountsaccountidadclientsadclientidcustomchannels-get
      parameters:
      - in: path
        name: accountId
        description: Account to which the ad client belongs
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
  /accounts/{accountId}/adclients/{adClientId}/customchannels/{customChannelId}:
    get:
      summary: Get Custom Channels
      description: Get the specified custom channel from the specified ad client.
      operationId: adexchangeseller.accounts.customchannels.get
      x-api-path-slug: accountsaccountidadclientsadclientidcustomchannelscustomchannelid-get
      parameters:
      - in: path
        name: accountId
        description: Account to which the ad client belongs
      - in: path
        name: adClientId
        description: Ad client which contains the custom channel
      - in: path
        name: customChannelId
        description: Custom channel to retrieve
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /accounts/{accountId}/adclients/{adClientId}/urlchannels:
    get:
      summary: Get URL Channels
      description: List all URL channels in the specified ad client for this Ad Exchange
        account.
      operationId: adexchangeseller.accounts.urlchannels.list
      x-api-path-slug: accountsaccountidadclientsadclientidurlchannels-get
      parameters:
      - in: path
        name: accountId
        description: Account to which the ad client belongs
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