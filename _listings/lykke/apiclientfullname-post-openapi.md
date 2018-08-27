---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Clientfullname
  version: 1.0.0
  description: Add api clientfullname.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Client/codes:
    get:
      summary: Get API Client Codes
      description: Get api client codes.
      operationId: ApiClientCodesGet
      x-api-path-slug: apiclientcodes-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Codes
    post:
      summary: Add API Client Codes
      description: Add api client codes.
      operationId: ApiClientCodesPost
      x-api-path-slug: apiclientcodes-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Codes
  /api/Client/keys/encodedmainkey:
    post:
      summary: Add API Client Keys Encodedmainkey
      description: Add api client keys encodedmainkey.
      operationId: ApiClientKeysEncodedmainkeyPost
      x-api-path-slug: apiclientkeysencodedmainkey-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Keys
      - Encodedmainkey
  /api/Client/balances/{baseAsset}:
    get:
      summary: Get API Client Balances Baseasset
      description: Get api client balances baseasset.
      operationId: ApiClientBalancesByBaseAssetGet
      x-api-path-slug: apiclientbalancesbaseasset-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: baseAsset
      responses:
        200:
          description: OK
      tags:
      - Client
      - Balances
      - Baseasset
  /api/Client/pushTxDialogOk:
    post:
      summary: Add API Client Pushtxdialogok
      description: Add api client pushtxdialogok.
      operationId: ApiClientPushTxDialogOkPost
      x-api-path-slug: apiclientpushtxdialogok-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Pushtxdialogok
  /api/Client/dictionary/{key}:
    get:
      summary: Get API Client Dictionary Key
      description: Get api client dictionary key.
      operationId: ApiClientDictionaryByKeyGet
      x-api-path-slug: apiclientdictionarykey-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
      - Key
    delete:
      summary: Delete API Client Dictionary Key
      description: Delete api client dictionary key.
      operationId: ApiClientDictionaryByKeyDelete
      x-api-path-slug: apiclientdictionarykey-delete
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
      - Key
  /api/Client/dictionary:
    put:
      summary: Put API Client Dictionary
      description: Put api client dictionary.
      operationId: ApiClientDictionaryPut
      x-api-path-slug: apiclientdictionary-put
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: keyValue
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
    post:
      summary: Add API Client Dictionary
      description: Add api client dictionary.
      operationId: ApiClientDictionaryPost
      x-api-path-slug: apiclientdictionary-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: keyValue
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
  /api/Client/properties/isUserFromUS:
    get:
      summary: Get API Client Properties Isuserfromus
      description: Get api client properties isuserfromus.
      operationId: ApiClientPropertiesIsUserFromUSGet
      x-api-path-slug: apiclientpropertiesisuserfromus-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Properties
      - Isuserfromus
    post:
      summary: Add API Client Properties Isuserfromus
      description: Add api client properties isuserfromus.
      operationId: ApiClientPropertiesIsUserFromUSPost
      x-api-path-slug: apiclientpropertiesisuserfromus-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Properties
      - Isuserfromus
  /api/Client/pendingActions:
    get:
      summary: Get API Client Pendingactions
      description: Get api client pendingactions.
      operationId: ApiClientPendingActionsGet
      x-api-path-slug: apiclientpendingactions-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Pendingactions
  /api/client/Dialogs:
    get:
      summary: Get API Client Dialogs
      description: Get api client dialogs.
      operationId: ApiClientDialogsGet
      x-api-path-slug: apiclientdialogs-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dialogs
    post:
      summary: Add API Client Dialogs
      description: Add api client dialogs.
      operationId: ApiClientDialogsPost
      x-api-path-slug: apiclientdialogs-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dialogs
  /api/ClientFirstNameLastName:
    post:
      summary: Add API Clientfirstnamelastname
      description: Add api clientfirstnamelastname.
      operationId: ApiClientFirstNameLastNamePost
      x-api-path-slug: apiclientfirstnamelastname-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clientfirstnamelastname
  /api/ClientFullName:
    post:
      summary: Add API Clientfullname
      description: Add api clientfullname.
      operationId: ApiClientFullNamePost
      x-api-path-slug: apiclientfullname-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: fullNameModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clientfullname
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