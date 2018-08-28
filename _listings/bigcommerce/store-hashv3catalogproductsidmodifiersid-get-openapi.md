---
swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 0
info:
  title: BigCommerce Retrieve a product modifier
  description: ""
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/catalog/products/{id}/modifiers:
    post:
      summary: Create a product modifier
      description: ""
      operationId: V3CatalogProductsModifiersByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidmodifiers-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Modifier
    get:
      summary: Retrieve an array of product modifiers
      description: ""
      operationId: V3CatalogProductsModifiersByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidmodifiers-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Array
      - Of
      - Product
      - Modifiers
  /{store_hash}/v3/catalog/products/{id}/modifiers/{id}:
    get:
      summary: Retrieve a product modifier
      description: ""
      operationId: V3CatalogProductsModifiersIdByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidmodifiersid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Product
      - Modifier
    put:
      summary: Update a product modifier
      description: ""
      operationId: V3CatalogProductsModifiersIdByStoreHashAndIdPut
      x-api-path-slug: store-hashv3catalogproductsidmodifiersid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Modifier
    delete:
      summary: Delete a product's modifier
      description: ""
      operationId: V3CatalogProductsModifiersIdByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidmodifiersid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Products
      - Modifier
  /{store_hash}/v3/catalog/products/{id}/modifiers/{id}/values/{id}/image:
    post:
      summary: Add an image to a modifier value
      description: "Add an image to a modifier value that will show on the storefront
        when it\u2019s selected"
      operationId: V3CatalogProductsModifiersIdValuesIdImageByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidmodifiersidvaluesidimage-post
      parameters:
      - in: path
        name: id
      - in: formData
        name: image_file
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Image
      - To
      - Modifier
      - Value
    delete:
      summary: Delete the image associated with a modifier
      description: Delete the image applied to show when the modifier value is selected
      operationId: V3CatalogProductsModifiersIdValuesIdImageByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidmodifiersidvaluesidimage-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Image
      - Associated
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