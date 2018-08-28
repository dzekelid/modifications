---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API Modify Cache Subnet Group
  version: 1.0.0
  description: Modifies an existing cache subnet group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAllowedNodeTypeModifications:
    get:
      summary: List Allowed Node Type Modifications
      description: |-
        Lists all available node types that you
                    can scale your Redis cluster's or replication group's current node type up to.
      operationId: listAllowedNodeTypeModifications
      x-api-path-slug: actionlistallowednodetypemodifications-get
      parameters:
      - in: query
        name: CacheClusterId
        description: The name of the cache cluster you want to scale up to a larger
          node instanced type
        type: string
      - in: query
        name: ReplicationGroupId
        description: The name of the replication group want to scale up to a larger
          node type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Node Type Modifications
  /?Action=ModifyCacheCluster:
    get:
      summary: Modify Cache Cluster
      description: Modifies the settings for a cache cluster.
      operationId: modifyCacheCluster
      x-api-path-slug: actionmodifycachecluster-get
      parameters:
      - in: query
        name: ApplyImmediately
        description: If true, this parameter causes the modifications in this request
          and any            pending modifications to be applied, asynchronously and
          as soon as possible, regardless            of the PreferredMaintenanceWindow
          setting for the cache cluster
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: This parameter is currently disabled
        type: string
      - in: query
        name: AZMode
        description: Specifies whether the new nodes in this Memcached cache cluster
          are all created in a             single Availability Zone or created across
          multiple Availability Zones
        type: string
      - in: query
        name: CacheClusterId
        description: The cache cluster identifier
        type: string
      - in: query
        name: CacheNodeIdsToRemove.CacheNodeId.N
        description: A list of cache node IDs to be removed
        type: string
      - in: query
        name: CacheNodeType
        description: A valid cache node type that you want to scale this cache cluster
          up to
        type: string
      - in: query
        name: CacheParameterGroupName
        description: The name of the cache parameter group to apply to this cache
          cluster
        type: string
      - in: query
        name: CacheSecurityGroupNames.CacheSecurityGroupName.N
        description: A list of cache security group names to authorize on this cache
          cluster
        type: string
      - in: query
        name: EngineVersion
        description: The upgraded version of the cache engine to be run on the cache
          nodes
        type: string
      - in: query
        name: NewAvailabilityZones.PreferredAvailabilityZone.N
        description: The list of Availability Zones where the new Memcached cache
          nodes are created
        type: string
      - in: query
        name: NotificationTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon SNS topic to which
          notifications are sent
        type: string
      - in: query
        name: NotificationTopicStatus
        description: The status of the Amazon SNS notification topic
        type: string
      - in: query
        name: NumCacheNodes
        description: The number of cache nodes that the cache cluster should have
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: Specifies the weekly time range during which maintenance   on
          the cluster is performed
        type: string
      - in: query
        name: SecurityGroupIds.SecurityGroupId.N
        description: Specifies the VPC Security Groups associated with the cache cluster
        type: string
      - in: query
        name: SnapshotRetentionLimit
        description: The number of days for which ElastiCache retains automatic cache
          cluster snapshots before            deleting them
        type: string
      - in: query
        name: SnapshotWindow
        description: The daily time range (in UTC) during which ElastiCache  begins
          taking a daily snapshot of            your cache cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Clusters
  /?Action=ModifyCacheParameterGroup:
    get:
      summary: Modify Cache Parameter Group
      description: |-
        Modifies the parameters of a cache
                    parameter group.
      operationId: modifyCacheParameterGroup
      x-api-path-slug: actionmodifycacheparametergroup-get
      parameters:
      - in: query
        name: CacheParameterGroupName
        description: The name of the cache parameter group to modify
        type: string
      - in: query
        name: ParameterNameValues.ParameterNameValue.N
        description: An array of parameter names and values for the parameter update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameter Groups
  /?Action=ModifyCacheSubnetGroup:
    get:
      summary: Modify Cache Subnet Group
      description: Modifies an existing cache subnet group.
      operationId: modifyCacheSubnetGroup
      x-api-path-slug: actionmodifycachesubnetgroup-get
      parameters:
      - in: query
        name: CacheSubnetGroupDescription
        description: A description of the cache subnet group
        type: string
      - in: query
        name: CacheSubnetGroupName
        description: The name for the cache subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: The EC2 subnet IDs for the cache subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups
  /?Action=ModifyReplicationGroup:
    get:
      summary: Modify Replication Group
      description: Modifies the settings for a replication group.
      operationId: modifyReplicationGroup
      x-api-path-slug: actionmodifyreplicationgroup-get
      parameters:
      - in: query
        name: ApplyImmediately
        description: If true, this parameter causes the modifications in this request
          and any            pending modifications to be applied, asynchronously and
          as soon as possible, regardless            of the PreferredMaintenanceWindow
          setting for the replication group
        type: string
      - in: query
        name: AutomaticFailoverEnabled
        description: Determines whether a read replica is automatically promoted to
          read/write primary if the existing primary encounters a failure
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: This parameter is currently disabled
        type: string
      - in: query
        name: CacheNodeType
        description: A valid cache node type that you want to scale this replication
          group to
        type: string
      - in: query
        name: CacheParameterGroupName
        description: The name of the cache parameter group to apply to all of the
          clusters in this replication group
        type: string
      - in: query
        name: CacheSecurityGroupNames.CacheSecurityGroupName.N
        description: A list of cache security group names to authorize for the clusters
          in this replication group
        type: string
      - in: query
        name: EngineVersion
        description: The upgraded version of the cache engine to be run on the cache
          clusters in the replication group
        type: string
      - in: query
        name: NotificationTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon SNS topic to which
          notifications are sent
        type: string
      - in: query
        name: NotificationTopicStatus
        description: The status of the Amazon SNS notification topic for the replication
          group
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: Specifies the weekly time range during which maintenance   on
          the cluster is performed
        type: string
      - in: query
        name: PrimaryClusterId
        description: For replication groups with a single primary,             if
          this parameter is specified, ElastiCache promotes the specified cluster
          in the specified replication group to the primary role
        type: string
      - in: query
        name: ReplicationGroupDescription
        description: A description for the replication group
        type: string
      - in: query
        name: ReplicationGroupId
        description: The identifier of the replication group to modify
        type: string
      - in: query
        name: SecurityGroupIds.SecurityGroupId.N
        description: Specifies the VPC Security Groups associated with the cache clusters
          in the replication group
        type: string
      - in: query
        name: SnapshotRetentionLimit
        description: The number of days for which ElastiCache retains automatic node
          group (shard) snapshots before            deleting them
        type: string
      - in: query
        name: SnapshottingClusterId
        description: The cache cluster ID that is used as the daily snapshot source
          for the replication group
        type: string
      - in: query
        name: SnapshotWindow
        description: The daily time range (in UTC) during which ElastiCache  begins
          taking a daily snapshot of            the node group (shard) specified by
          SnapshottingClusterId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Groups
  /?Action=ResetCacheParameterGroup:
    get:
      summary: Reset Cache Parameter Group
      description: |-
        Modifies the parameters of a cache
                    parameter group to the engine or system default value.
      operationId: resetCacheParameterGroup
      x-api-path-slug: actionresetcacheparametergroup-get
      parameters:
      - in: query
        name: CacheParameterGroupName
        description: The name of the cache parameter group to reset
        type: string
      - in: query
        name: ParameterNameValues.ParameterNameValue.N
        description: An array of parameter names to reset to their default values
        type: string
      - in: query
        name: ResetAllParameters
        description: If true,             all parameters in the cache parameter group
          are reset to their default values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameter Groups
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