---
swagger: "2.0"
x-collection-name: NPR
x-complete: 0
info:
  title: NPR Retrieve the most recent promo audio heard by the logged-in user
  description: Gets the most recently played promo for which the user has neither
    tapped through the promo or listened to the target story.
  termsOfService: http://dev.npr.org/develop/terms-of-use
  contact:
    name: NPR One Enterprise Team
    url: http://dev.npr.org
    email: NPROneEnterprise@npr.org
  version: 1.0.0
host: api.npr.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listening/v2/promo/recommendations:
    get:
      summary: Retrieve the most recent promo audio heard by the logged-in user
      description: Gets the most recently played promo for which the user has neither
        tapped through the promo or listened to the target story.
      operationId: getPromo
      x-api-path-slug: listeningv2promorecommendations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - News
      - Listening
      - Promo
      - Recommendations
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