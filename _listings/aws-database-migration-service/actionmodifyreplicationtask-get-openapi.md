---
swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 0
info:
  title: AWS Database Migration Service API Modify Replication Task
  version: 1.0.0
  description: Modifies the specified replication task.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyEndpoint:
    get:
      summary: Modify Endpoint
      description: Modifies the specified endpoint.
      operationId: modifyEndpoint
      x-api-path-slug: actionmodifyendpoint-get
      parameters:
      - in: query
        name: CertificateArn
        description: The Amazon Resource Name (ARN) of the certificate used for SSL
          connection
        type: string
      - in: query
        name: DatabaseName
        description: The name of the endpoint database
        type: string
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: EndpointIdentifier
        description: The database endpoint identifier
        type: string
      - in: query
        name: EndpointType
        description: The type of endpoint
        type: string
      - in: query
        name: EngineName
        description: The type of engine for the endpoint
        type: string
      - in: query
        name: ExtraConnectionAttributes
        description: Additional attributes associated with the connection
        type: string
      - in: query
        name: Password
        description: The password to be used to login to the endpoint database
        type: string
      - in: query
        name: Port
        description: The port used by the endpoint database
        type: string
      - in: query
        name: ServerName
        description: The name of the server where the endpoint database resides
        type: string
      - in: query
        name: SslMode
        description: The SSL mode to be used
        type: string
      - in: query
        name: Username
        description: The user name to be used to login to the endpoint database
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=ModifyReplicationInstance:
    get:
      summary: Modify Replication Instance
      description: Modifies the replication instance to apply new settings.
      operationId: modifyReplicationInstance
      x-api-path-slug: actionmodifyreplicationinstance-get
      parameters:
      - in: query
        name: AllocatedStorage
        description: The amount of storage (in gigabytes) to be allocated for the
          replication instance
        type: string
      - in: query
        name: AllowMajorVersionUpgrade
        description: Indicates that major version upgrades are allowed
        type: string
      - in: query
        name: ApplyImmediately
        description: Indicates whether the changes should be applied immediately or
          during the next maintenance window
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor version upgrades will be applied automatically     to
          the replication instance during the maintenance window
        type: string
      - in: query
        name: EngineVersion
        description: The engine version number of the replication instance
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the replication instance is a Multi-AZ deployment
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which system maintenance
          can occur, which might result in an outage
        type: string
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance
        type: string
      - in: query
        name: ReplicationInstanceClass
        description: The compute and memory capacity of the replication instance
        type: string
      - in: query
        name: ReplicationInstanceIdentifier
        description: The replication instance identifier
        type: string
      - in: query
        name: VpcSecurityGroupIds
        description: Specifies the VPC security group to be used with the replication
          instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=ModifyReplicationSubnetGroup:
    get:
      summary: Modify Replication Subnet Group
      description: Modifies the settings for the specified replication subnet group.
      operationId: modifyReplicationSubnetGroup
      x-api-path-slug: actionmodifyreplicationsubnetgroup-get
      parameters:
      - in: query
        name: ReplicationSubnetGroupDescription
        description: The description of the replication instance subnet group
        type: string
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The name of the replication instance subnet group
        type: string
      - in: query
        name: SubnetIds
        description: A list of subnet IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Subnet Groups
  /?Action=ModifyReplicationTask:
    get:
      summary: Modify Replication Task
      description: Modifies the specified replication task.
      operationId: modifyReplicationTask
      x-api-path-slug: actionmodifyreplicationtask-get
      parameters:
      - in: query
        name: CdcStartTime
        description: The start time for the Change Data Capture (CDC) operation
        type: string
      - in: query
        name: MigrationType
        description: The migration type
        type: string
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Name (ARN) of the replication task
        type: string
      - in: query
        name: ReplicationTaskIdentifier
        description: The replication task identifier
        type: string
      - in: query
        name: ReplicationTaskSettings
        description: JSON file that contains settings for the task, such as target
          metadata settings
        type: string
      - in: query
        name: TableMappings
        description: The path of the JSON file that contains the table mappings
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
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