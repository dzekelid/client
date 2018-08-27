---
name: moltin
x-slug: moltin
description: The comprehensive eCommerce API infrastructure for any platform. Moltin
  handles data storage and eCommerce logic in the cloud so that you can focus on creating
  great customer experiences.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/moltin-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Client
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/moltin/apis.md
specificationVersion: "0.14"
apis:
- name: Moltin - Client credential token
  x-api-slug: oauthaccess-token-post
  description: |-
    An access token will allow you to make requests for your store. We support two types of token: `client_credentials` and `implicit`.

    An `implcit` token is typically used for situations where you are requesting data on the client side and you are exposing your public key - such as JavaScript - and adding your client secret would be disastrous. You will only be able to perform a limited number of operations on the API endpoints.

    A `client_credentials` token is used when the credentials are not publicly exposed, usually a server side language such as PHP. You will be able to perform all operations on API endpoints.

    A `refresh_token` type can be used when you have an existing token which you would like to extend the life of. When your `grant_type` is `refresh_token` you must also provide the original token in the `refresh_token` field.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/moltin-logo.png
  humanURL: https://moltin.com
  baseURL: https://api.moltin.com//
  tags: Commerce, Target, Commerce, Stack Network, Retail, Kiosk, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/moltin/oauthaccess-token-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://mocklab.api.gallery.streamdata.io
- type: x-api-stack
  url: http://moltin.stack.network
- type: x-base
  url: https://api.molt.in/
- type: x-blog
  url: https://molt.in/blog
- type: x-developer
  url: https://molt.in/developers
- type: x-documentation
  url: https://docs.moltin.com/
- type: x-email
  url: support@molt.in
- type: x-github
  url: https://github.com/moltin
- type: x-postman
  url: https://www.getpostman.com/collections/e9bdcde0ccb5a08640e6
- type: x-pricing
  url: https://moltin.com/pricing
- type: x-twitter
  url: https://twitter.com/moltin
- type: x-website
  url: https://moltin.com
- type: x-website
  url: https://molt.in/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---