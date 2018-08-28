---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Modify D B Parameter Group
  version: 1.0.0
  description: Modifies the parameters of a DB parameter group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyDBClusterParameterGroup:
    get:
      summary: Modify D B Cluster Parameter Group
      description: Modifies the parameters of a DB cluster parameter group.
      operationId: modifydbclusterparametergroup
      x-api-path-slug: actionmodifydbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to modify
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: A list of parameters in the DB cluster parameter group to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=ModifyDBInstance:
    get:
      summary: Modify D B Instance
      description: Modifies settings for a DB instance.
      operationId: modifydbinstance
      x-api-path-slug: actionmodifydbinstance-get
      parameters:
      - in: query
        name: AllocatedStorage
        description: The new storage capacity of the RDS instance
        type: string
      - in: query
        name: AllowMajorVersionUpgrade
        description: Indicates that major version upgrades are allowed
        type: string
      - in: query
        name: ApplyImmediately
        description: Specifies whether the modifications in this request and        any
          pending modifications are asynchronously applied        as soon as possible,
          regardless of the        PreferredMaintenanceWindow setting for the DB instance
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor version upgrades will be applied automatically    to
          the DB instance during the maintenance window
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days to retain automated backups
        type: string
      - in: query
        name: CACertificateIdentifier
        description: Indicates the certificate that needs to be associated with the
          instance
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the DB instance to snapshots of the
          DB instance; otherwise false
        type: string
      - in: query
        name: DBInstanceClass
        description: The new compute and memory capacity of the DB instance
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group to apply to the DB instance
        type: string
      - in: query
        name: DBPortNumber
        description: The port number on which the database accepts connections
        type: string
      - in: query
        name: DBSecurityGroups.DBSecurityGroupName.N
        description: A list of DB security groups to authorize on this DB instance
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The new DB subnet group for the DB instance
        type: string
      - in: query
        name: Domain
        description: The Active Directory Domain to move the instance to
        type: string
      - in: query
        name: DomainIAMRoleName
        description: The name of the IAM role to use when making API calls to the
          Directory Service
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the database engine to upgrade to
        type: string
      - in: query
        name: Iops
        description: The new Provisioned IOPS (I/O operations per second) value for
          the RDS instance
        type: string
      - in: query
        name: LicenseModel
        description: The license model for the DB instance
        type: string
      - in: query
        name: MasterUserPassword
        description: The new password for the DB instance master user
        type: string
      - in: query
        name: MonitoringInterval
        description: The interval, in seconds, between points when Enhanced Monitoring
          metrics are collected for the DB instance
        type: string
      - in: query
        name: MonitoringRoleArn
        description: The ARN for the IAM role that permits RDS to send enhanced monitoring
          metrics to CloudWatch Logs
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the DB instance is a Multi-AZ deployment
        type: string
      - in: query
        name: NewDBInstanceIdentifier
        description: The new DB instance identifier for the DB instance when renaming
          a DB            instance
        type: string
      - in: query
        name: OptionGroupName
        description: Indicates that the DB instance should be associated with the
          specified option group
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled,        as determined by the BackupRetentionPeriod
          parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which system maintenance
          can occur, which might result in an outage
        type: string
      - in: query
        name: PromotionTier
        description: A value that specifies the order in which an Aurora Replica is
          promoted to the primary instance       after a failure of the existing primary
          instance
        type: string
      - in: query
        name: PubliclyAccessible
        description: Boolean value that indicates if the DB instance has a publicly
          resolvable DNS name
        type: string
      - in: query
        name: StorageType
        description: Specifies the storage type to be associated with the DB instance
        type: string
      - in: query
        name: TdeCredentialArn
        description: The ARN from the Key Store with which to associate the instance
          for TDE encryption
        type: string
      - in: query
        name: TdeCredentialPassword
        description: The password for the given ARN from the Key Store in order to
          access the device
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of EC2 VPC security groups to authorize on this DB instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=ModifyDBParameterGroup:
    get:
      summary: Modify D B Parameter Group
      description: Modifies the parameters of a DB parameter group.
      operationId: modifydbparametergroup
      x-api-path-slug: actionmodifydbparametergroup-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of parameter names, values, and the apply method for
          the parameter update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=ModifyDBSubnetGroup:
    get:
      summary: Modify D B Subnet Group
      description: Modifies an existing DB subnet group.
      operationId: modifydbsubnetgroup
      x-api-path-slug: actionmodifydbsubnetgroup-get
      parameters:
      - in: query
        name: DBSubnetGroupDescription
        description: The description for the DB subnet group
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The name for the DB subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: The EC2 subnet IDs for the DB subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet Groups
  /?Action=ModifyEventSubscription:
    get:
      summary: Modify Event Subscription
      description: Modifies an existing RDS event notification subscription.
      operationId: modifyeventsubscription
      x-api-path-slug: actionmodifyeventsubscription-get
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value; set to true to activate the subscription
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: A list of event categories for a SourceType that you want to
          subscribe to
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the SNS topic created for event
          notification
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=ModifyOptionGroup:
    get:
      summary: Modify Option Group
      description: Modifies an existing option group.
      operationId: modifyoptiongroup
      x-api-path-slug: actionmodifyoptiongroup-get
      parameters:
      - in: query
        name: ApplyImmediately
        description: Indicates whether the changes should be applied immediately,
          or during the next maintenance window for each instance associated with
          the option group
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to be modified
        type: string
      - in: query
        name: OptionsToInclude.OptionConfiguration.N
        description: Options in this list are added to the option group or, if already
          present, the specified configuration is used to update the existing configuration
        type: string
      - in: query
        name: OptionsToRemove.member.N
        description: Options in this list are removed from the option group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=ResetDBClusterParameterGroup:
    get:
      summary: Reset D B Cluster Parameter Group
      description: Modifies the parameters of a DB cluster parameter group to the
        default value.
      operationId: resetdbclusterparametergroup
      x-api-path-slug: actionresetdbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to reset
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: A list of parameter names in the DB cluster parameter group to
          reset to the default values
        type: string
      - in: query
        name: ResetAllParameters
        description: A value that is set to true to reset all parameters in the DB
          cluster parameter group       to their default values, and false otherwise
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=ResetDBParameterGroup:
    get:
      summary: Reset D B Parameter Group
      description: Modifies the parameters of a DB parameter group to the engine/system
        default value.
      operationId: resetdbparametergroup
      x-api-path-slug: actionresetdbparametergroup-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of parameter names, values, and the apply method for
          the parameter update
        type: string
      - in: query
        name: ResetAllParameters
        description: Specifies whether (true) or not (false) to reset all parameters        in
          the DB parameter group to default values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=ModifyDBCluster:
    get:
      summary: Modify D B Cluster
      description: Modify a setting for an Amazon Aurora DB cluster.
      operationId: modifydbcluster
      x-api-path-slug: actionmodifydbcluster-get
      parameters:
      - in: query
        name: ApplyImmediately
        description: A value that specifies whether the modifications in this request
          and      any pending modifications are asynchronously applied      as soon
          as possible, regardless of the      PreferredMaintenanceWindow setting for
          the DB cluster
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days for which automated backups are retained
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The DB cluster identifier for the cluster being modified
        type: string
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to use for the DB
          cluster
        type: string
      - in: query
        name: MasterUserPassword
        description: The new password for the master database user
        type: string
      - in: query
        name: NewDBClusterIdentifier
        description: The new DB cluster identifier for the DB cluster when renaming
          a DB cluster
        type: string
      - in: query
        name: OptionGroupName
        description: A value that indicates that the DB cluster should be associated
          with the specified option group
        type: string
      - in: query
        name: Port
        description: The port number on which the DB cluster accepts connections
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created            if
          automated backups are enabled,            using the BackupRetentionPeriod
          parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A lst of VPC security groups that the DB cluster will belong
          to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ModifyDBClusterSnapshotAttribute:
    get:
      summary: Modify D B Cluster Snapshot Attribute
      description: Adds an attribute and values to, or removes an attribute and values
        from, a manual DB cluster snapshot.
      operationId: modifydbclustersnapshotattribute
      x-api-path-slug: actionmodifydbclustersnapshotattribute-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the DB cluster snapshot attribute to modify
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier for the DB cluster snapshot to modify the attributes
          for
        type: string
      - in: query
        name: ValuesToAdd.AttributeValue.N
        description: A list of DB cluster snapshot attributes to add to the attribute
          specified by AttributeName
        type: string
      - in: query
        name: ValuesToRemove.AttributeValue.N
        description: A list of DB cluster snapshot attributes to remove from the attribute
          specified by AttributeName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
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