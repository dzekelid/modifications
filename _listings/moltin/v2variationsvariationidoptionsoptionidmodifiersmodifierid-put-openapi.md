---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Update Product Modifier
  description: Update product modifier.
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
  /v2/variations/{variationID}/options/{optionID}/modifiers/{modifierID}:
    put:
      summary: Update Product Modifier
      description: Update product modifier.
      operationId: V2VariationsOptionsModifiersModifierIDByVariationIDAndOptionIDPut
      x-api-path-slug: v2variationsvariationidoptionsoptionidmodifiersmodifierid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: modifierID
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Modifier
    delete:
      summary: Delete Product Modifier
      description: Delete product modifier.
      operationId: V2VariationsOptionsModifiersModifierIDByVariationIDAndOptionIDDelete
      x-api-path-slug: v2variationsvariationidoptionsoptionidmodifiersmodifierid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: modifierID
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Modifier
  /v2/variations/{variationID}/options/{optionID}/modifiers:
    post:
      summary: Create Product Modifier
      description: Create product modifier.
      operationId: V2VariationsOptionsModifiersByVariationIDAndOptionIDPost
      x-api-path-slug: v2variationsvariationidoptionsoptionidmodifiers-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Modifier
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