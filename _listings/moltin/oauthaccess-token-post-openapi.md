---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Client credential token
  description: |-
    An access token will allow you to make requests for your store. We support two types of token: `client_credentials` and `implicit`.

    An `implcit` token is typically used for situations where you are requesting data on the client side and you are exposing your public key - such as JavaScript - and adding your client secret would be disastrous. You will only be able to perform a limited number of operations on the API endpoints.

    A `client_credentials` token is used when the credentials are not publicly exposed, usually a server side language such as PHP. You will be able to perform all operations on API endpoints.

    A `refresh_token` type can be used when you have an existing token which you would like to extend the life of. When your `grant_type` is `refresh_token` you must also provide the original token in the `refresh_token` field.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth/access_token:
    post:
      summary: Client credential token
      description: |-
        An access token will allow you to make requests for your store. We support two types of token: `client_credentials` and `implicit`.

        An `implcit` token is typically used for situations where you are requesting data on the client side and you are exposing your public key - such as JavaScript - and adding your client secret would be disastrous. You will only be able to perform a limited number of operations on the API endpoints.

        A `client_credentials` token is used when the credentials are not publicly exposed, usually a server side language such as PHP. You will be able to perform all operations on API endpoints.

        A `refresh_token` type can be used when you have an existing token which you would like to extend the life of. When your `grant_type` is `refresh_token` you must also provide the original token in the `refresh_token` field.
      operationId: OauthAccessTokenPost2
      x-api-path-slug: oauthaccess-token-post
      parameters:
      - in: header
        name: Accept
      - in: formData
        name: client_id
        description: Replace with the values from your dashboard
      - in: formData
        name: client_secret
        description: Replace with the values from your dashboard
      - in: header
        name: Content-Type
      - in: formData
        name: grant_type
        description: client_credentials | implicit | refresh_token
      responses:
        200:
          description: Successful response
      tags:
      - Client
      - Credential
      - Token
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