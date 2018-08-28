---
swagger: "2.0"
x-collection-name: BBC
x-complete: 0
info:
  title: BBC Nitro Get raw promotion
  description: Get raw promotion
  termsOfService: http://www.bbc.co.uk/terms/
  contact:
    name: Open Nitro Project
    url: http://developer.bbc.co.uk/
    email: nitro@bbc.co.uk
  version: 1.0.0
host: programmes.api.bbc.com
basePath: /nitro/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /promotions:
    get:
      summary: Discover metadata for content promotions
      description: Details of short-term editorially curated "promotions", for instance
        those programmes featured on iPlayer today
      operationId: listPromotions
      x-api-path-slug: promotions-get
      parameters:
      - in: query
        name: context
        description: filter for subset of promotions belonging to a given context
      - in: query
        name: mixin
        description: 'Mixins:* related_links: mixin to return information about related
          links to a promotion'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for promotions by partner ID
      - in: query
        name: partner_pid
        description: filter for promotions by partner PID
      - in: query
        name: pid
        description: filter for subset of promotions having given PID
      - in: query
        name: promoted_by
        description: filter for subset of promotions having given promoted by
      - in: query
        name: promoted_for
        description: filter for subset of promotions having given promoted for
      - in: query
        name: q
        description: filter for subset of promotions matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: status
        description: filter for subset of promotions with status
      responses:
        200:
          description: OK
      tags:
      - Promotions
  /v1/promotions/{pid}:
    get:
      summary: Get raw promotion
      description: Get raw promotion
      operationId: Get_Raw_promotion
      x-api-path-slug: v1promotionspid-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Promotions
      - Pid
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