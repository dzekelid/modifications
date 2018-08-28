swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
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