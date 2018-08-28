swagger: "2.0"
x-collection-name: Quovo
x-complete: 1
info:
  title: Quovo API v3
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /connections/{connection_id}:
    put:
      summary: Modify a connection
      description: Modifies an existing connection.
      operationId: ConnectionsByConnectionIdPut
      x-api-path-slug: connectionsconnection-id-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: connection_id
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Modify
      - Connection
  /users/{user_id}:
    put:
      summary: Modify a user
      description: Modifies an existing User.
      operationId: UsersByUserIdPut
      x-api-path-slug: usersuser-id-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Modify
      - User
  /accounts/{account_id}:
    put:
      summary: Update an account
      description: Modifies an existing account.
      operationId: AccountsByAccountIdPut
      x-api-path-slug: accountsaccount-id-put
      parameters:
      - in: path
        name: account_id
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Account