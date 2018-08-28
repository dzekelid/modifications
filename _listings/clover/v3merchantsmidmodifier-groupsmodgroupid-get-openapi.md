---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Get a modifier group
  version: 1.0.0
  description: Get a single modifier group by it's UUID
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/modifications:
    post:
      summary: Apply a modification to a line item
      description: 'Create a modification, a record of a modifier as it exists at
        the time it is applied to the lineItem. To view current modifications use
        an ''expand=modifications'' query parameter on the lineItem. To learn more
        about applying a modification see: https://docs.clover.com/build/working-with-orders/#add-item-modifiers'
      operationId: ApplyModification
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemidmodifications-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Modifications
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/modifications/{modificationId}:
    delete:
      summary: Remove a modification from a line item
      description: Delete a modification by UUID, removing the record of an applied
        modification
      operationId: RemoveModification
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modificationId
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Modifications
      - ModificationId
  /v3/merchants/{mId}/modifier_groups/{modGroupId}:
    get:
      summary: Get a modifier group
      description: Get a single modifier group by it's UUID
      operationId: GetModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
    post:
      summary: Update a modifier group
      description: Update a modifier group. In order to add modifiers use the create
        modifiers endpoint.
      operationId: UpdateModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
    delete:
      summary: Delete a modifier group
      description: Delete an existing modifier group, identified by UUID. This also
        deletes all modifiers within that group.
      operationId: DeleteModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
  /v3/merchants/{mId}/modifier_groups/{modGroupId}/modifiers:
    get:
      summary: Get all modifiers belonging to a single modifier group
      description: Get an array containing the modifiers in a single modifier group.
      operationId: GetModifiersByGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, price, name, alternateName, id,
          modifierGroup'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
    post:
      summary: Create a modifier
      description: Create a modifier object belonging to the modifier group identified
        in the URL.
      operationId: CreateModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
  /v3/merchants/{mId}/modifier_groups/{modGroupId}/modifiers/{modId}:
    get:
      summary: Get a single modifier
      description: Get a single modifier by it's group, and it's UUID
      operationId: GetModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      - in: path
        name: modId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
      - ModId
    post:
      summary: Update a single modifier
      description: Update a modifier. Note that once it has been created, it is not
        possible to change a modifier's group.
      operationId: UpdateModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      - in: path
        name: modId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
      - ModId
    delete:
      summary: Delete a single modifier
      description: Delete a single modifier by it's UUID
      operationId: DeleteModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      - in: path
        name: modId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
      - ModId
  /v3/merchants/{mId}/modifier_groups:
    get:
      summary: Get all modifier groups
      description: These groupings are the categories different modifiers belong to.
        Modifier groups can be made available for specific inventory Items by creating
        an item to modifier group association.
      operationId: GetModifierGroups
      x-api-path-slug: v3merchantsmidmodifier-groups-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
    post:
      summary: Create a modifier group
      description: Create a new modifier group. Modifiers can be associated with a
        modifier group after it has been created.
      operationId: CreateModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
  /v3/merchants/{mId}/item_modifier_groups:
    post:
      summary: Create or delete item to modifier group associations
      description: 'Create or delete one or more association objects (item modifier
        groups). Modifiers can only be applied to items associated with that modifier''s
        group. Learn more about object associations here: https://docs.clover.com/build/web-api/#object-associations'
      operationId: CreateOrDeleteItemModifierGroups
      x-api-path-slug: v3merchantsmiditem-modifier-groups-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Modifier
      - Groups
  /v3/merchants/{mId}/modifier_group_sort_orders:
    post:
      summary: Update the priorities for a collection of up to 200 modifier groups
        at a time
      description: Update the priorities for a collection of up to 200 modifier groups
        at a time.
      operationId: UpdateModifierGroupSortOrders
      x-api-path-slug: v3merchantsmidmodifier-group-sort-orders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Group
      - Sort
      - Orders
  /v3/merchants/{mId}/modifiers:
    get:
      summary: Get all modifiers
      description: Get all modifiers regardless of their modifier group.
      operationId: GetModifiers
      x-api-path-slug: v3merchantsmidmodifiers-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, price, name, alternateName, id,
          modifierGroup'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifiers
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