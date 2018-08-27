swagger: "2.0"
x-collection-name: Authentiq Connect
x-complete: 1
info:
  title: Authentiq Connect
  description: authentiq-connect-oauth-2-0-and-openid-connect-api-reference-learn-about-authentiq-idhttpswww-authentiq-com-or-check-out-the-authentiq-connecthttpsdevelopers-authentiq-com-developer-documentation-
  termsOfService: https://www.authentiq.com/tos/
  contact:
    name: Team Authentiq
    url: https://www.authentiq.com/
    email: hello@authentiq.com
  version: "1.0"
host: connect.authentiq.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /client:
    get:
      summary: List clients
      description: Retrieve a list of clients.
      operationId: client
      x-api-path-slug: client-get
      responses:
        200:
          description: OK
      tags:
      - Client
    post:
      summary: Register a client
      description: |-
        Register a new client with this Authentiq Connect provider.

        This endpoint is compatible with [OIDC's Client Registration](http://openid.net/specs/openid-connect-registration-1_0.html) extension.

        See also:
        - [OIDC Client Registration Endpoint](http://openid.net/specs/openid-connect-registration-1_0.html#ClientRegistration)
      operationId: createClient
      x-api-path-slug: client-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Client
  /client/{client_id}:
    delete:
      summary: Delete a client
      description: Delete a previously registered client.
      operationId: clientClient_id
      x-api-path-slug: clientclient-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Client
      - Client
      - Id
    get:
      summary: View a client
      description: |-
        Retrieve the configuration of a previously registered client.

        See also:
        - [OIDC Client Configuration Endpoint](http://openid.net/specs/openid-connect-registration-1_0.html#ClientConfigurationEndpoint)
      operationId: getClient
      x-api-path-slug: clientclient-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Client
      - Client
      - Id
    put:
      summary: Update a client
      description: |-
        Update the configuration of a previously registered client.

        See also:
        - [OIDC Client Configuration Endpoint](http://openid.net/specs/openid-connect-registration-1_0.html#ClientConfigurationEndpoint)
      operationId: updateClient
      x-api-path-slug: clientclient-id-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Client
      - Client
      - Id
  /{client_id}/iframe:
    get:
      summary: Include a session iframe
      description: |-
        An OpenID Connect Session Management iframe to facilitate e.g. single sign-on or remote logouts.

        The iframe implements the OIDC postMessage-based [change notification protocol](http://openid.net/specs/openid-connect-session-1_0.html#ChangeNotification) via which a client can receive notifications about session state changes.

        See also:
        - [OIDC OP iframe](http://openid.net/specs/openid-connect-session-1_0.html#OPiframe)
      operationId: authorizeIframe
      x-api-path-slug: client-idiframe-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Client
      - Id
      - Iframe