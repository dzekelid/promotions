---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Post Promotions
  description: ""
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /promotions.json:
    get:
      summary: Get Promotions
      description: ""
      operationId: getPromotions.json
      x-api-path-slug: promotions-json-get
      parameters:
      - in: query
        name: limit
        description: 'Promotions list restriction (default: 50 | max: 200)'
      - in: query
        name: No Name
      - in: query
        name: page
        description: 'Promotions list page (default: 1)'
      responses:
        200:
          description: OK
      tags:
      - Promotions
      - Json
    post:
      summary: Post Promotions
      description: ""
      operationId: postPromotions.json
      x-api-path-slug: promotions-json-post
      parameters:
      - in: body
        name: body
        description: Promotion parameters
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Promotions
      - Json
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