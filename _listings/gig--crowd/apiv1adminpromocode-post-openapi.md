---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Admin Promocode
  version: 1.0.0
  description: Post admin promocode.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/event/promo/{eventId}:
    post:
      summary: Post Event Promo Eventid
      description: Post event promo eventid.
      operationId: postApiV1EventPromoEvent
      x-api-path-slug: apiv1eventpromoeventid-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Event
      - Promo
      - Eventid
    delete:
      summary: Delete Event Promo Eventid
      description: Delete event promo eventid.
      operationId: deleteApiV1EventPromoEvent
      x-api-path-slug: apiv1eventpromoeventid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Promo
      - Eventid
  /api/v1/admin/promocode/generate:
    get:
      summary: Get Admin Promocode Generate
      description: Get admin promocode generate.
      operationId: getApiV1AdminPromocodeGenerate
      x-api-path-slug: apiv1adminpromocodegenerate-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Generate
  /api/v1/admin/promocode/{page}:
    get:
      summary: Get Admin Promocode Page
      description: Get admin promocode page.
      operationId: getApiV1AdminPromocodePage
      x-api-path-slug: apiv1adminpromocodepage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.used
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Page
  /api/v1/admin/promocode:
    post:
      summary: Post Admin Promocode
      description: Post admin promocode.
      operationId: postApiV1AdminPromocode
      x-api-path-slug: apiv1adminpromocode-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
  /api/v1/admin/promocode/{promoCodeId}:
    put:
      summary: Put Admin Promocode Promocodeid
      description: Put admin promocode promocodeid.
      operationId: putApiV1AdminPromocodePromocode
      x-api-path-slug: apiv1adminpromocodepromocodeid-put
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: promoCodeId
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Promocodeid
    delete:
      summary: Delete Admin Promocode Promocodeid
      description: Delete admin promocode promocodeid.
      operationId: deleteApiV1AdminPromocodePromocode
      x-api-path-slug: apiv1adminpromocodepromocodeid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: promoCodeId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Promocodeid
  /api/v1/payment/promocode/price:
    post:
      summary: Post Payment Promocode Price
      description: Post payment promocode price.
      operationId: postApiV1PaymentPromocodePrice
      x-api-path-slug: apiv1paymentpromocodeprice-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Promocode
      - Price
  /api/v1/payment/promocode/{requestId}:
    post:
      summary: Post Payment Promocode Requestid
      description: Post payment promocode requestid.
      operationId: postApiV1PaymentPromocodeRequest
      x-api-path-slug: apiv1paymentpromocoderequestid-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: requestId
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Promocode
      - Requestid
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