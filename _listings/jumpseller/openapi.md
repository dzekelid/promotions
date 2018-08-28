swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 1
info:
  title: Jumpseller
  description: explore-all-our-endpoints-with-your-own-set-of-of-access-tokens--all-changes-affect-your-production-jumpseller-store-
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
  /promotions/{id}.json:
    delete:
      summary: Delete Promotions
      description: ""
      operationId: deletePromotions.json
      x-api-path-slug: promotionsid-json-delete
      parameters:
      - in: path
        name: id
        description: Id of the Promotion
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Promotions
      - Id
      - Json
    get:
      summary: Get Promotions
      description: ""
      operationId: getPromotions.json
      x-api-path-slug: promotionsid-json-get
      parameters:
      - in: path
        name: id
        description: Id of the Promotion
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Promotions
      - Id
      - Json
    put:
      summary: Put Promotions
      description: ""
      operationId: putPromotions.json
      x-api-path-slug: promotionsid-json-put
      parameters:
      - in: body
        name: body
        description: Promotion parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Id of the Promotion
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Promotions
      - Id
      - Json