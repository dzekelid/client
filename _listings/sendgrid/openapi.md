swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clients/{client_type}/stats:
    get:
      summary: Get Clients Client Type Stats
      description: |-
        **This endpoint allows you to retrieve your email statistics segmented by a specific client type.**

        **We only store up to 7 days of email activity in our database.** By default, 500 items will be returned per request via the Advanced Stats API endpoints.

        ## Available Client Types
        - phone
        - tablet
        - webmail
        - desktop

        Advanced Stats provide a more in-depth view of your email statistics and the actions taken by your recipients. You can segment these statistics by geographic location, device type, client type, browser, and mailbox provider. For more information about statistics, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/index.html).
      operationId: clients.client_type.stats.get
      x-api-path-slug: clientsclient-typestats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: No Name
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Clients
      - Client
      - Type
      - Stats