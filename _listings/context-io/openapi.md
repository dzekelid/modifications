---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}:
    put:
      summary: Put Accounts
      description: Modifies a given account.
      operationId: modifyAccount_
      x-api-path-slug: accountsid-put
      parameters:
      - in: query
        name: first_name
        description: First name of the account holder
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: last_name
        description: Last name of the account holder
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}/sources/{label}:
    put:
      summary: Put Accounts Sources Label
      description: Modifies a data source on a given account.
      operationId: modifyAccountSource_
      x-api-path-slug: accountsidsourceslabel-put
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      - in: query
        name: password
        description: New password for this source
      - in: query
        name: provider_consumer_key
        description: The OAuth consumer key used to obtain the the token and token
          secret above for that account
      - in: query
        name: provider_token
        description: An OAuth token obtained from the IMAP account provider to be
          used to authentify on this email account
      - in: query
        name: provider_token_secret
        description: An OAuth token secret obtained from the IMAP account provider
          to be used to authentify on this email account
      - in: query
        name: service_level
        description: Changes the service level for the source
      - in: query
        name: status
        description: If the status of the source is TEMP_DISABLED or DISABLED
      - in: query
        name: sync_period
        description: Changes the period at which the Context
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
---