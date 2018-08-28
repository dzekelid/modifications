---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API Update Device Pool
  version: 1.0.0
  description: Modifies the name, description, and rules in a device pool given the
    attributes and the pool ARN.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateDevicePool:
    get:
      summary: Update Device Pool
      description: Modifies the name, description, and rules in a device pool given
        the attributes and the pool ARN.
      operationId: updateDevicePool
      x-api-path-slug: actionupdatedevicepool-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resourc Name (ARN) of the Device Farm device pool
          you wish to update
        type: string
      - in: query
        name: description
        description: A description of the device pool you wish to update
        type: string
      - in: query
        name: name
        description: A string representing the name of the device pool you wish to
          update
        type: string
      - in: query
        name: rules
        description: Represents the rules you wish to modify for the device pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
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