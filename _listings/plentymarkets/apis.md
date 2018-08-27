---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Client
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - List accounting locations of a client
  x-api-slug: restaccountingstoresplentyidlocations-get
  description: Lists accounting locations of a client. The plenty ID of the client
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/plentymarkets/restaccountingstoresplentyidlocations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/plentymarkets/restaccountingstoresplentyidlocations-get-openapi.md
- name: plentymarkets REST-API - Activate a client (store)
  x-api-slug: restitemssales-pricesidonline-stores-post
  description: Activates a client (store) for a sales price. The ID of the sales price
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/plentymarkets/restitemssales-pricesidonline-stores-post-openapi.md
- name: plentymarkets REST-API - Deactivate a client (store)
  x-api-slug: restitemssales-pricesidonline-storeswebstoreid-delete
  description: Deactivates a client (store) for a sales price. The ID of the sales
    price and the ID of the client (store) must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/plentymarkets/restitemssales-pricesidonline-storeswebstoreid-delete-openapi.md
- name: plentymarkets REST-API - Link a client to a variation
  x-api-slug: restitemsidvariationsvariationidvariation-clients-post
  description: Creates a link between a client (store) and a variation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/plentymarkets/restitemsidvariationsvariationidvariation-clients-post-openapi.md
- name: plentymarkets REST-API - Unlink a client from a variation
  x-api-slug: restitemsidvariationsvariationidvariation-clientsplentyid-delete
  description: Deletes the link between a client (store) and a variation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/plentymarkets/restitemsidvariationsvariationidvariation-clientsplentyid-delete-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration for the standard accounting
    location of a client
  x-api-slug: restvatstandard-get
  description: Gets the VAT configuration currently used for the country of the standard
    accounting location of a client (store). The ID of the client (store) must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/plentymarkets/restvatstandard-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---