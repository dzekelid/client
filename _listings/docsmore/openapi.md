swagger: "2.0"
x-collection-name: Docsmore
x-complete: 1
info:
  title: Docsmore API 2.1
  description: alt-texthttpswww-docsmore-comwpcontentuploads201802docsmoreapi-png-titleh3create-a-developer-account-at-docsmore-io-and-start-unleashing-the-power-of-docsmore-into-your-own-applications--to-make-it-easier-we-have-provided-client-libraries-and-sdk-in-several-languages-for-you-to-get-started-and-hit-the-ground-running-in-no-time-h3brbrh4note-if-you-dont-see-api-setting-under-top-right-menu-that-means-you-will-need-to-be-a-developer-account--please-contact-supportdocsmore-com-and-a-customer-service-expert-will-switch-your-account-to-developer-account--h4brbrh5just-head-over-to-httpsdocsmore-io-and-sign-up-for-your-30-days-trial-h5
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /getclientdocs:
    post:
      summary: Get List of Client Documents By Document ID
      description: In order to export as PDf, you will need to have client document
        ID available for that specific document you are looking to download.
      operationId: GetclientdocsPost
      x-api-path-slug: getclientdocs-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Client
      - Documents
      - Document
      - ID
  /rawdata:
    post:
      summary: Returns raw data response as json FOR SINGLE CLIENT DOC
      description: This API call gets you underlying raw data of the document. All
        you need to do is supply Auth token and Document Key as part of the call
      operationId: RawdataPost
      x-api-path-slug: rawdata-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Raw
      - Data
      - Response
      - As
      - Json
      - FOR
      - SINGLE
      - CLIENT
      - DOC