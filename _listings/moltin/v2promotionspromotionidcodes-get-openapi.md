---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Get a list of promotion codes
  description: Get a list of promotion codes.
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
    post:
      summary: Create a promotion
      description: Create a promotion.
      operationId: V2PromotionsPost
      x-api-path-slug: v2promotions-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
  /v2/promotions/{promotionID}/codes:
    get:
      summary: Get a list of promotion codes
      description: Get a list of promotion codes.
      operationId: V2PromotionsCodesByPromotionIDGet
      x-api-path-slug: v2promotionspromotionidcodes-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
      - Codes
    post:
      summary: Create promotion codes
      description: Create promotion codes.
      operationId: V2PromotionsCodesByPromotionIDPost
      x-api-path-slug: v2promotionspromotionidcodes-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
      - Codes
  /v2/promotions/{promotionID}:
    get:
      summary: Get a promotion
      description: Get a promotion.
      operationId: V2PromotionsByPromotionIDGet
      x-api-path-slug: v2promotionspromotionid-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
    put:
      summary: Update promotion
      description: Update promotion.
      operationId: V2PromotionsByPromotionIDPut
      x-api-path-slug: v2promotionspromotionid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
    delete:
      summary: Delete Promotion
      description: Delete promotion.
      operationId: V2PromotionsByPromotionIDDelete
      x-api-path-slug: v2promotionspromotionid-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
  /v2/carts/123456/items:
    post:
      summary: Add a promotion to a cart
      description: |-
        Update an existing item in a cart. The updated cart contents are returned if the call is successful.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart **OR** productID.

        When updating custom itesm you must use the identifier in the cart - you can update more properties of a custom cart item.
      operationId: V2Carts123456ItemsPost2
      x-api-path-slug: v2carts123456items-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
      - To
      - Cart
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