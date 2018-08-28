---
swagger: "2.0"
x-collection-name: Google Books
x-complete: 0
info:
  title: Google Books API Dismiss Promotion Offer
  description: Dismiss promotion offer
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /promooffer/accept:
    post:
      summary: Accept Promotion Offer
      description: Accept promotion offer
      operationId: books.promooffer.accept
      x-api-path-slug: promoofferaccept-post
      parameters:
      - in: query
        name: androidId
        description: device android_id
      - in: query
        name: device
        description: device device
      - in: query
        name: manufacturer
        description: device manufacturer
      - in: query
        name: model
        description: device model
      - in: query
        name: offerId
      - in: query
        name: product
        description: device product
      - in: query
        name: serial
        description: device serial
      - in: query
        name: volumeId
        description: Volume id to exercise the offer
      responses:
        200:
          description: OK
      tags:
      - Promotion
  /promooffer/dismiss:
    post:
      summary: Dismiss Promotion Offer
      description: Dismiss promotion offer
      operationId: books.promooffer.dismiss
      x-api-path-slug: promoofferdismiss-post
      parameters:
      - in: query
        name: androidId
        description: device android_id
      - in: query
        name: device
        description: device device
      - in: query
        name: manufacturer
        description: device manufacturer
      - in: query
        name: model
        description: device model
      - in: query
        name: offerId
        description: Offer to dimiss
      - in: query
        name: product
        description: device product
      - in: query
        name: serial
        description: device serial
      responses:
        200:
          description: OK
      tags:
      - Promotion
  /promooffer/get:
    get:
      summary: Get Promotion Offer
      description: Returns a list of promo offers available to the user
      operationId: books.promooffer.get
      x-api-path-slug: promoofferget-get
      parameters:
      - in: query
        name: androidId
        description: device android_id
      - in: query
        name: device
        description: device device
      - in: query
        name: manufacturer
        description: device manufacturer
      - in: query
        name: model
        description: device model
      - in: query
        name: product
        description: device product
      - in: query
        name: serial
        description: device serial
      responses:
        200:
          description: OK
      tags:
      - Promotion
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