---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get a VAT configuration for the standard accounting location
    of a client
  description: Gets the VAT configuration currently used for the country of the standard
    accounting location of a client (store). The ID of the client (store) must be
    specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounting/stores/{plentyId}/locations:
    get:
      summary: List accounting locations of a client
      description: Lists accounting locations of a client. The plenty ID of the client
        must be specified.
      operationId: getRestAccountingStoresPlentyLocations
      x-api-path-slug: restaccountingstoresplentyidlocations-get
      parameters:
      - in: query
        name: locationId
        description: The plenty ID
      - in: path
        name: plentyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Accounting
      - Locations
      - Of
      - Client
  /rest/items/sales_prices/{id}/online_stores:
    post:
      summary: Activate a client (store)
      description: Activates a client (store) for a sales price. The ID of the sales
        price must be specified.
      operationId: postRestItemsSalesPricesOnlineStores
      x-api-path-slug: restitemssales-pricesidonline-stores-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/online_stores
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Client
      - (store)
  /rest/items/sales_prices/{id}/online_stores/{webstoreId}:
    delete:
      summary: Deactivate a client (store)
      description: Deactivates a client (store) for a sales price. The ID of the sales
        price and the ID of the client (store) must be specified.
      operationId: deleteRestItemsSalesPricesOnlineStoresWebstore
      x-api-path-slug: restitemssales-pricesidonline-storeswebstoreid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: webstoreId
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Client
      - (store)
  /rest/items/{id}/variations/{variationId}/variation_clients:
    post:
      summary: Link a client to a variation
      description: Creates a link between a client (store) and a variation.
      operationId: postRestItemsVariationsVariationVariationClients
      x-api-path-slug: restitemsidvariationsvariationidvariation-clients-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_clients
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Client
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_clients/{plentyId}:
    delete:
      summary: Unlink a client from a variation
      description: Deletes the link between a client (store) and a variation.
      operationId: deleteRestItemsVariationsVariationVariationClientsPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-clientsplentyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Unlink
      - Client
      - From
      - Variation
  /rest/vat/standard:
    get:
      summary: Get a VAT configuration for the standard accounting location of a client
      description: Gets the VAT configuration currently used for the country of the
        standard accounting location of a client (store). The ID of the client (store)
        must be specified.
      operationId: getRestVatStandard
      x-api-path-slug: restvatstandard-get
      parameters:
      - in: query
        name: plentyId
        description: The plenty ID of the client (store)
      - in: query
        name: startedAt
        description: The date in the W3C format when the vat configuration went into
          effect
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configurationthe
      - Standard
      - Accounting
      - Location
      - Of
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