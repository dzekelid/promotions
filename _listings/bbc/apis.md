---
name: BBC
x-slug: bbc
description: Breaking news, sport, TV, radio and a whole lot more. The BBC informs,
  educates and entertains - wherever you are, whatever your age.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28554-bbc-nitro.jpg
x-kinRank: "7"
x-alexaRank: "93"
tags: Promotions
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/promotions/master/_listings/bbc/apis.md
specificationVersion: "0.14"
apis:
- name: BBC Nitro - Discover metadata for content promotions
  x-api-slug: promotions-get
  description: Details of short-term editorially curated "promotions", for instance
    those programmes featured on iPlayer today
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28554-bbc-nitro.jpg
  humanURL: http://www.bbc.com/
  baseURL: https://programmes.api.bbc.com//nitro/api
  tags: Media, API Provider, Broadcasts, Profiles, Publish, General Data, Historical
    Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/promotions/master/_listings/bbc/promotions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/promotions/master/_listings/bbc/promotions-get-openapi.md
- name: BBC Nitro - Get raw promotion
  x-api-slug: v1promotionspid-get
  description: Get raw promotion
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28554-bbc-nitro.jpg
  humanURL: http://www.bbc.com/
  baseURL: https://programmes.api.bbc.com//nitro/api
  tags: Media, API Provider, Broadcasts, Profiles, Publish, General Data, Historical
    Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/promotions/master/_listings/bbc/v1promotionspid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/promotions/master/_listings/bbc/v1promotionspid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://barclays.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bbc.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bbc-news
- type: x-email
  url: dataprotection@bbc.com
- type: x-email
  url: bbcworldwidelearning@bbc.com
- type: x-twitter
  url: https://twitter.com/BBCNews
- type: x-website
  url: http://www.bbc.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---