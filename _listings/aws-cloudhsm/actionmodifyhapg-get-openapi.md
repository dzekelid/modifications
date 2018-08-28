---
swagger: "2.0"
x-collection-name: AWS CloudHSM
x-complete: 0
info:
  title: AWS CloudHSM API Modify HAPG
  version: 1.0.0
  description: Modifies an existing high-availability partition group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyHapg:
    get:
      summary: Modify HAPG
      description: Modifies an existing high-availability partition group.
      operationId: modifyHapg
      x-api-path-slug: actionmodifyhapg-get
      parameters:
      - in: query
        name: HapgArn
        description: The ARN of the high-availability partition group to modify
        type: string
      - in: query
        name: Label
        description: The new label for the high-availability partition group
        type: string
      - in: query
        name: PartitionSerialList
        description: The list of partition serial numbers to make members of the high-availability
          partition      group
        type: string
      responses:
        200:
          description: OK
      tags:
      - High-Availability Partition Group
  /?Action=ModifyHsm:
    get:
      summary: Modify HSM
      description: Modifies an HSM.
      operationId: modifyHsm
      x-api-path-slug: actionmodifyhsm-get
      parameters:
      - in: query
        name: EniIp
        description: The new IP address for the elastic network interface (ENI) attached
          to the      HSM
        type: string
      - in: query
        name: ExternalId
        description: The new external ID
        type: string
      - in: query
        name: HsmArn
        description: The ARN of the HSM to modify
        type: string
      - in: query
        name: IamRoleArn
        description: The new IAM role ARN
        type: string
      - in: query
        name: SubnetId
        description: The new identifier of the subnet that the HSM is in
        type: string
      - in: query
        name: SyslogIp
        description: The new IP address for the syslog monitoring server
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=ModifyLunaClient:
    get:
      summary: Modify Luna Client
      description: Modifies the certificate used by the client.
      operationId: modifyLunaClient
      x-api-path-slug: actionmodifylunaclient-get
      parameters:
      - in: query
        name: Certificate
        description: The new certificate for the client
        type: string
      - in: query
        name: ClientArn
        description: The ARN of the client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
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