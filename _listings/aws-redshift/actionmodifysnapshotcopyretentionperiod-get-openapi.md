---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Modify Snapshot Copy Retention Period
  version: 1.0.0
  description: |-
    Modifies the number of days to retain automated snapshots in the destination region
                after they are copied from the source region.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyCluster:
    get:
      summary: Modify Cluster
      description: Modifies the settings for a cluster.
      operationId: modifyCluster
      x-api-path-slug: actionmodifycluster-get
      parameters:
      - in: query
        name: AllowVersionUpgrade
        description: If true, major version upgrades will be applied automatically
          to the            cluster during the maintenance window
        type: string
      - in: query
        name: AutomatedSnapshotRetentionPeriod
        description: The number of days that automated snapshots are retained
        type: string
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the cluster to be modified
        type: string
      - in: query
        name: ClusterParameterGroupName
        description: The name of the cluster parameter group to apply to this cluster
        type: string
      - in: query
        name: ClusterSecurityGroups.ClusterSecurityGroupName.N
        description: A list of cluster security groups to be authorized on this cluster
        type: string
      - in: query
        name: ClusterType
        description: The new cluster type
        type: string
      - in: query
        name: ClusterVersion
        description: The new version number of the Amazon Redshift engine to upgrade
          to
        type: string
      - in: query
        name: ElasticIp
        description: The Elastic IP (EIP) address for the cluster
        type: string
      - in: query
        name: EnhancedVpcRouting
        description: An option that specifies whether to create the cluster with enhanced
          VPC routing            enabled
        type: string
      - in: query
        name: HsmClientCertificateIdentifier
        description: Specifies the name of the HSM client certificate the Amazon Redshift
          cluster uses to            retrieve the data encryption keys stored in an
          HSM
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: Specifies the name of the HSM configuration that contains the
          information the            Amazon Redshift cluster can use to retrieve and
          store keys in an HSM
        type: string
      - in: query
        name: MasterUserPassword
        description: The new password for the cluster master user
        type: string
      - in: query
        name: NewClusterIdentifier
        description: The new identifier for the cluster
        type: string
      - in: query
        name: NodeType
        description: The new node type of the cluster
        type: string
      - in: query
        name: NumberOfNodes
        description: The new number of nodes of the cluster
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which system maintenance
          can occur, if            necessary
        type: string
      - in: query
        name: PubliclyAccessible
        description: If true, the cluster can be accessed from a public network
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of virtual private cloud (VPC) security groups to be associated
          with the            cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ModifyClusterIamRoles:
    get:
      summary: Modify Cluster Iam Roles
      description: |-
        Modifies the list of AWS Identity and Access Management (IAM) roles that can be
                    used by the cluster to access other AWS services.
      operationId: modifyClusterIamRoles
      x-api-path-slug: actionmodifyclusteriamroles-get
      parameters:
      - in: query
        name: AddIamRoles.IamRoleArn.N
        description: Zero or more IAM roles to associate with the cluster
        type: string
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the cluster for which you want to associate
          or            disassociate IAM roles
        type: string
      - in: query
        name: RemoveIamRoles.IamRoleArn.N
        description: Zero or more IAM roles in ARN format to disassociate from the
          cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster IAM Roles
  /?Action=ModifyClusterParameterGroup:
    get:
      summary: Modify Cluster Parameter Group
      description: Modifies the parameters of a parameter group.
      operationId: modifyClusterParameterGroup
      x-api-path-slug: actionmodifyclusterparametergroup-get
      parameters:
      - in: query
        name: ParameterGroupName
        description: The name of the parameter group to be modified
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of parameters to be modified
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=ModifyClusterSubnetGroup:
    get:
      summary: Modify Cluster Subnet Group
      description: Modifies a cluster subnet group to include the specified list of
        VPC subnets.
      operationId: modifyClusterSubnetGroup
      x-api-path-slug: actionmodifyclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the subnet group to be modified
        type: string
      - in: query
        name: Description
        description: A text description of the subnet group to be modified
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: An array of VPC subnet IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=ModifyEventSubscription:
    get:
      summary: Modify Event Subscription
      description: Modifies an existing Amazon Redshift event notification subscription.
      operationId: modifyEventSubscription
      x-api-path-slug: actionmodifyeventsubscription-get
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value indicating if the subscription is enabled
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: Specifies the Amazon Redshift event categories to be published
          by the event notification            subscription
        type: string
      - in: query
        name: Severity
        description: Specifies the Amazon Redshift event severity to be published
          by the event notification            subscription
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the SNS topic to be used by
          the event            notification subscription
        type: string
      - in: query
        name: SourceIds.SourceId.N
        description: A list of one or more identifiers of Amazon Redshift source objects
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the modified Amazon Redshift event notification subscription
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=ModifySnapshotCopyRetentionPeriod:
    get:
      summary: Modify Snapshot Copy Retention Period
      description: |-
        Modifies the number of days to retain automated snapshots in the destination region
                    after they are copied from the source region.
      operationId: modifySnapshotCopyRetentionPeriod
      x-api-path-slug: actionmodifysnapshotcopyretentionperiod-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the cluster for which you want to change
          the retention            period for automated snapshots that are copied
          to a destination region
        type: string
      - in: query
        name: RetentionPeriod
        description: The number of days to retain automated snapshots in the destination
          region after            they are copied from the source region
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
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