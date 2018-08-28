swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 1
info:
  title: Coinbase API
  description: the-coinbase-v2-api
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}:
    put:
      summary: Update account
      description: "Modifies user\u2019s account name."
      operationId: modifies-users-account-name
      x-api-path-slug: accountsaccount-id-put
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: body
        name: account_properties
        description: Properties to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Account