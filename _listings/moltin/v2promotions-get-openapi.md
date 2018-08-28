---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Get a list of promotions
  description: Get a list of promotions.
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
  /v2/promotions:
    get:
      summary: Get a list of promotions
      description: Get a list of promotions.
      operationId: V2PromotionsGet
      x-api-path-slug: v2promotions-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Promotions
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