---
name: AWS Cognito
x-slug: aws-cognito
description: Amazon Cognito lets you easily add user sign-up and sign-in to your mobile
  and web apps. With Amazon Cognito, you also have the options to authenticate users
  through social identity providers such as Facebook, Twitter, or Amazon, with SAML
  identity solutions, or by using your own identity system. In addition, Amazon Cognito
  enables you to save data locally on users devices, allowing your applications to
  work even when the devices are offline. You can then synchronize data across users
  devices so that their app experience remains consistent regardless of the device
  they use. With Amazon Cognito, you can focus on creating great app experiences instead
  of worrying about building, securing, and scaling a solution to handle user management,
  authentication, and sync across devices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Client
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Cognito Merged API - Create User Pool Client
  x-api-slug: actioncreateuserpoolclient-get
  description: Creates the user pool client.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https:///
  tags: Amazon Web Services, Authentication, Social, Facebook, Twitter, Stack Network,
    API Service Provider, API Service Provider, API Provider, Identities, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actioncreateuserpoolclient-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actioncreateuserpoolclient-get-openapi.md
- name: AWS Cognito Merged API - Delete User Pool Client
  x-api-slug: actiondeleteuserpoolclient-get
  description: Allows the developer to delete the user pool client.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https:///
  tags: Amazon Web Services, Authentication, Social, Facebook, Twitter, Stack Network,
    API Service Provider, API Service Provider, API Provider, Identities, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actiondeleteuserpoolclient-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actiondeleteuserpoolclient-get-openapi.md
- name: AWS Cognito Merged API - Describe User Pool Client
  x-api-slug: actiondescribeuserpoolclient-get
  description: |-
    Client method for returning the configuration information and metadata of the
                specified user pool client.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https:///
  tags: Amazon Web Services, Authentication, Social, Facebook, Twitter, Stack Network,
    API Service Provider, API Service Provider, API Provider, Identities, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actiondescribeuserpoolclient-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actiondescribeuserpoolclient-get-openapi.md
- name: AWS Cognito Merged API - List User Pool Clients
  x-api-slug: actionlistuserpoolclients-get
  description: Lists the clients that have been created for the specified user pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https:///
  tags: Amazon Web Services, Authentication, Social, Facebook, Twitter, Stack Network,
    API Service Provider, API Service Provider, API Provider, Identities, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actionlistuserpoolclients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actionlistuserpoolclients-get-openapi.md
- name: AWS Cognito Merged API - Update User Pool Client
  x-api-slug: actionupdateuserpoolclient-get
  description: |-
    Allows the developer to update the specified user pool client and password
                policy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https:///
  tags: Amazon Web Services, Authentication, Social, Facebook, Twitter, Stack Network,
    API Service Provider, API Service Provider, API Provider, Identities, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actionupdateuserpoolclient-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/client/master/_listings/aws-cognito/actionupdateuserpoolclient-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.codedeploy.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.cognito.stack.network
- type: x-blog
  url: https://aws.amazon.com/cognito/dev-resources/#blogposts
- type: x-documentation
  url: http://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/Welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/cognitoidentity/latest/APIReference/Welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/cognitosync/latest/APIReference/Welcome.html
- type: x-faq
  url: http://aws.amazon.com/cognito/faqs
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=173
- type: x-pricing
  url: http://aws.amazon.com/cognito/pricing
- type: x-sdk
  url: https://aws.amazon.com/cognito/dev-resources/#documentation
- type: x-slides
  url: https://aws.amazon.com/cognito/dev-resources/#slides
- type: x-videos
  url: https://aws.amazon.com/cognito/dev-resources/#videos
- type: x-website
  url: https://aws.amazon.com/cognito/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---