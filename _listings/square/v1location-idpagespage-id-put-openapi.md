---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Modifies the details of a Favorites page in Square Register.
  description: Modifies the details of a Favorites page in Square Register.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/items/{item_id}:
    get:
      summary: Provides the details for a single item, including associated modifier
        lists and fees.
      description: Provides the details for a single item, including associated modifier
        lists and fees.
      operationId: RetrieveItem
      x-api-path-slug: v1location-iditemsitem-id-get
      parameters:
      - in: path
        name: item_id
        description: The items ID
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Item
      - ""
      - Including
      - Associated
      - Modifier
      - Lists
      - Fees
    put:
      summary: Modifies the core details of an existing item.
      description: Modifies the core details of an existing item.
      operationId: UpdateItem
      x-api-path-slug: v1location-iditemsitem-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: item_id
        description: The ID of the item to modify
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Core
      - Details
      - Of
      - Existing
      - Item
  /v1/{location_id}/items/{item_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      description: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      operationId: RemoveModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to remove the modifier list from
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to remove
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Modifier
      - List
      - Association
      - From
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - "No"
      - Longer
      - Be
      - Applied
      - To
      - Item
    put:
      summary: Associates a modifier list with an item, meaning modifier options from
        the list can be applied to the item.
      description: Associates a modifier list with an item, meaning modifier options
        from the list can be applied to the item.
      operationId: ApplyModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-put
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to add the modifier list to
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to apply
      responses:
        200:
          description: OK
      tags:
      - Associates
      - Modifier
      - List
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - Be
      - Applied
      - To
      - Item
  /v1/{location_id}/modifier-lists:
    get:
      summary: Lists all of a location's modifier lists.
      description: Lists all of a location's modifier lists.
      operationId: ListModifierLists
      x-api-path-slug: v1location-idmodifierlists-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list modifier lists for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Modifier
      - Lists
    post:
      summary: Creates an item modifier list and at least one modifier option for
        it.
      description: Creates an item modifier list and at least one modifier option
        for it.
      operationId: CreateModifierList
      x-api-path-slug: v1location-idmodifierlists-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create a modifier list for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Modifier
      - List
      - At
      - Least
      - Modifier
      - Optionit
  /v1/{location_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Deletes an existing item modifier list and all modifier options associated
        with it.
      description: Deletes an existing item modifier list and all modifier options
        associated with it.
      operationId: DeleteModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Modifier
      - List
      - ""
      - Modifier
      - Options
      - Associated
      - It
    get:
      summary: Provides the details for a single modifier list.
      description: Provides the details for a single modifier list.
      operationId: RetrieveModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The modifier lists ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Modifier
      - List
    put:
      summary: Modifies the details of an existing item modifier list.
      description: Modifies the details of an existing item modifier list.
      operationId: UpdateModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Modifier
      - List
  /v1/{location_id}/modifier-lists/{modifier_list_id}/modifier-options:
    post:
      summary: Creates an item modifier option and adds it to a modifier list.
      description: Creates an item modifier option and adds it to a modifier list.
      operationId: CreateModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptions-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Modifier
      - Option
      - Adds
      - It
      - To
      - Modifier
      - List
  /v1/{location_id}/modifier-lists/{modifier_list_id}/modifier-options/{modifier_option_id}:
    delete:
      summary: Deletes an existing item modifier option from a modifier list.
      description: Deletes an existing item modifier option from a modifier list.
      operationId: DeleteModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptionsmodifier-option-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      - in: path
        name: modifier_option_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Modifier
      - Option
      - From
      - Modifier
      - List
    put:
      summary: Modifies the details of an existing item modifier option.
      description: Modifies the details of an existing item modifier option.
      operationId: UpdateModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptionsmodifier-option-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      - in: path
        name: modifier_option_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Modifier
      - Option
  /v1/me/roles/{role_id}:
    put:
      summary: Modifies the details of an employee role.
      description: Modifies the details of an employee role.
      operationId: UpdateEmployeeRole
      x-api-path-slug: v1merolesrole-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: role_id
        description: The ID of the role to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Employee
      - Role
  /v1/me/timecards/{timecard_id}:
    put:
      summary: Modifies a timecard's details. This creates an API_EDIT event for the
        timecard. You can view a timecard's event history with the List Timecard Events
        endpoint.
      description: Modifies a timecard's details. This creates an API_EDIT event for
        the timecard. You can view a timecard's event history with the List Timecard
        Events endpoint.
      operationId: UpdateTimecard
      x-api-path-slug: v1metimecardstimecard-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: timecard_id
        description: TThe ID of the timecard to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Timecards
      - Details
      - ""
      - This
      - Creates
      - EDIT
      - Eventthe
      - Timecard
      - ""
      - You
      - Can
      - View
      - Timecards
      - Event
      - History
      - List
      - Timecard
      - Events
      - Endpoint
  /v1/{location_id}/categories/{category_id}:
    put:
      summary: Modifies the details of an existing item category.
      description: Modifies the details of an existing item category.
      operationId: UpdateCategory
      x-api-path-slug: v1location-idcategoriescategory-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: category_id
        description: The ID of the category to edit
      - in: path
        name: location_id
        description: The ID of the categorys associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Category
  /v1/{location_id}/discounts/{discount_id}:
    put:
      summary: Modifies the details of an existing discount.
      description: Modifies the details of an existing discount.
      operationId: UpdateDiscount
      x-api-path-slug: v1location-iddiscountsdiscount-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discount_id
        description: The ID of the discount to edit
      - in: path
        name: location_id
        description: The ID of the categorys associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Discount
  /v1/{location_id}/fees/{fee_id}:
    put:
      summary: Modifies the details of an existing fee (tax).
      description: Modifies the details of an existing fee (tax).
      operationId: UpdateFee
      x-api-path-slug: v1location-idfeesfee-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fee_id
        description: The ID of the fee to edit
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Fee
      - (tax)
  /v1/{location_id}/items/{item_id}/variations/{variation_id}:
    put:
      summary: Modifies the details of an existing item variation.
      description: Modifies the details of an existing item variation.
      operationId: UpdateVariation
      x-api-path-slug: v1location-iditemsitem-idvariationsvariation-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: item_id
        description: The ID of the item to modify
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: variation_id
        description: The ID of the variation to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Variation
  /v1/{location_id}/pages/{page_id}:
    put:
      summary: Modifies the details of a Favorites page in Square Register.
      description: Modifies the details of a Favorites page in Square Register.
      operationId: UpdatePage
      x-api-path-slug: v1location-idpagespage-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Favorites
      - Page
      - In
      - Square
      - Register
  /v1/{location_id}/pages/{page_id}/cells:
    put:
      summary: Modifies a cell of a Favorites page in Square Register.
      description: Modifies a cell of a Favorites page in Square Register.
      operationId: UpdatePageCell
      x-api-path-slug: v1location-idpagespage-idcells-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page the cell belongs to
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Cell
      - Of
      - Favorites
      - Page
      - In
      - Square
      - Register
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