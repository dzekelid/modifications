---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Modify Spot Fleet Request
  version: 1.0.0
  description: Modifies the specified Spot fleet request
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeReservedInstancesModifications:
    get:
      summary: Describe Reserved Instances Modifications
      description: Describes the modifications made to your Reserved Instances.
      operationId: describereservedinstancesmodifications
      x-api-path-slug: actiondescribereservedinstancesmodifications-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone in which the Reserved Instance can be used
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: IncludeMarketplace
        description: Include Reserved Instance Marketplace offerings in the response
        type: string
      - in: query
        name: InstanceTenancy
        description: The tenancy of the instances covered by the reservation
        type: string
      - in: query
        name: InstanceType
        description: The instance type that the reservation will cover (for example,
          m1
        type: string
      - in: query
        name: MaxDuration
        description: The maximum duration (in seconds) to filter when searching for
          offerings
        type: string
      - in: query
        name: MaxInstanceCount
        description: The maximum number of instances to filter when searching for
          offerings
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: MinDuration
        description: The minimum duration (in seconds) to filter when searching for
          offerings
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      - in: query
        name: OfferingClass
        description: The offering class of the Reserved Instance
        type: string
      - in: query
        name: OfferingType
        description: The Reserved Instance offering type
        type: string
      - in: query
        name: ProductDescription
        description: The Reserved Instance product platform description
        type: string
      - in: query
        name: ReservedInstancesOfferingId.N
        description: One or more Reserved Instances offering IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=ModifyIdentityIdFormat:
    get:
      summary: Modify Identity Id Format
      description: |-
        Modifies the ID format of a resource for a specified IAM user, IAM role, or the root
              user for an account; or all IAM users, IAM roles, and the root user for an account.
      operationId: modifyidentityidformat
      x-api-path-slug: actionmodifyidentityidformat-get
      parameters:
      - in: query
        name: Resource
        description: 'The type of resource: instance | reservation |        snapshot
          | volume'
        type: string
      - in: query
        name: UseLongIds
        description: Indicate whether the resource should use longer IDs (17-character
          IDs)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Format
  /?Action=ModifyIdFormat:
    get:
      summary: Modify Id Format
      description: Modifies the ID format for the specified resource on a per-region
        basis.
      operationId: modifyidformat
      x-api-path-slug: actionmodifyidformat-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: RouteTableId
        description: The ID of the route table
        type: string
      - in: query
        name: SubnetId
        description: The ID of the subnet
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Format
  /?Action=ModifyImageAttribute:
    get:
      summary: Modify Image Attribute
      description: Modifies the specified attribute of the specified AMI.
      operationId: modifyimageattribute
      x-api-path-slug: actionmodifyimageattribute-get
      parameters:
      - in: query
        name: Architecture
        description: The architecture of the AMI
        type: string
      - in: query
        name: BlockDeviceMapping.N
        description: One or more block device mapping entries
        type: string
      - in: query
        name: Description
        description: A description for your AMI
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EnaSupport
        description: Set to true to enable enhanced networking with ENA for the AMI
          and any instances that you launch from the AMI
        type: string
      - in: query
        name: ImageLocation
        description: The full path to your AMI manifest in Amazon S3 storage
        type: string
      - in: query
        name: KernelId
        description: The ID of the kernel
        type: string
      - in: query
        name: Name
        description: A name for your AMI
        type: string
      - in: query
        name: RamdiskId
        description: The ID of the RAM disk
        type: string
      - in: query
        name: RootDeviceName
        description: The name of the root device (for example, /dev/sda1, or/dev/xvda)
        type: string
      - in: query
        name: SriovNetSupport
        description: Set to simple to enable enhanced networking with the Intel 82599
          Virtual Function interface for the AMI and any instances that you launch
          from the AMI
        type: string
      - in: query
        name: VirtualizationType
        description: The type of virtualization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Image
  /?Action=ModifyInstanceAttribute:
    get:
      summary: Modify Instance Attribute
      description: Modifies the specified attribute of the specified instance.
      operationId: modifyinstanceattribute
      x-api-path-slug: actionmodifyinstanceattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=ModifyNetworkInterfaceAttribute:
    get:
      summary: Modify Network Interface Attribute
      description: Modifies the specified network interface attribute.
      operationId: modifynetworkinterfaceattribute
      x-api-path-slug: actionmodifynetworkinterfaceattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: SourceDestCheck
        description: The source/destination checking attribute
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network Interface
  /?Action=ModifyReservedInstances:
    get:
      summary: Modify Reserved Instances
      description: Modifies the Availability Zone, instance count, instance type,
        or network platform (EC2-Classic or EC2-VPC) of your Standard Reserved Instances.
      operationId: modifyreservedinstances
      x-api-path-slug: actionmodifyreservedinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceCount
        description: The number of Reserved Instances to purchase
        type: string
      - in: query
        name: LimitPrice
        description: Specified for Reserved Instance Marketplace offerings to limit
          the total order and ensure that the Reserved Instances are not purchased
          at unexpected prices
        type: string
      - in: query
        name: ReservedInstancesOfferingId
        description: The ID of the Reserved Instance offering to purchase
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance
  /?Action=ModifySpotFleetRequest:
    get:
      summary: Modify Spot Fleet Request
      description: Modifies the specified Spot fleet request
      operationId: modifyspotfleetrequest
      x-api-path-slug: actionmodifyspotfleetrequest-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: SpotFleetRequestConfig
        description: The configuration for the Spot fleet request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Fleet
  /?Action=ModifySubnetAttribute:
    get:
      summary: Modify Subnet Attribute
      description: Modifies a subnet attribute.
      operationId: modifysubnetattribute
      x-api-path-slug: actionmodifysubnetattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: ResourceId.N
        description: The IDs of one or more resources to tag
        type: string
      - in: query
        name: Tag.N
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet
  /?Action=ModifyVolumeAttribute:
    get:
      summary: Modify Volume Attribute
      description: Modifies a volume attribute.
      operationId: modifyvolumeattribute
      x-api-path-slug: actionmodifyvolumeattribute-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute to reset
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volume
  /?Action=ModifyVpcAttribute:
    get:
      summary: Modify Vpc Attribute
      description: Modifies the specified attribute of the specified VPC.
      operationId: modifyvpcattribute
      x-api-path-slug: actionmodifyvpcattribute-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the request
        type: string
      - in: query
        name: DeliverLogsPermissionArn
        description: The ARN for the IAM role thats used to post flow logs to a CloudWatch
          Logs log group
        type: string
      - in: query
        name: LogGroupName
        description: The name of the CloudWatch log group
        type: string
      - in: query
        name: ResourceId.N
        description: One or more subnet, network interface, or VPC IDs
        type: string
      - in: query
        name: ResourceType
        description: The type of resource on which to create the flow log
        type: string
      - in: query
        name: TrafficType
        description: The type of traffic to log
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC
  /?Action=ModifyVpcEndpoint:
    get:
      summary: Modify Vpc Endpoint
      description: Modifies attributes of a specified VPC endpoint.
      operationId: modifyvpcendpoint
      x-api-path-slug: actionmodifyvpcendpoint-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: VpcPeeringConnectionId
        description: The ID of the VPC peering connection
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC Endpoint
  /?Action=ModifyVpcPeeringConnectionOptions:
    get:
      summary: Modify Vpc Peering Connection Options
      description: Modifies the VPC peering connection options on one side of a VPC
        peering connection.
      operationId: modifyvpcpeeringconnectionoptions
      x-api-path-slug: actionmodifyvpcpeeringconnectionoptions-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: VpcPeeringConnectionId
        description: The ID of the VPC peering connection
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC Peering Connection
  /?Action=ModifyHosts:
    get:
      summary: Modify Hosts
      description: Modify the auto-placement setting of a Dedicated Host.
      operationId: modifyhosts
      x-api-path-slug: actionmodifyhosts-get
      parameters:
      - in: query
        name: Affinity
        description: The new affinity setting for the instance
        type: string
      - in: query
        name: HostId
        description: The ID of the Dedicated Host that the instance will have affinity
          with
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance that you are modifying
        type: string
      - in: query
        name: Tenancy
        description: The tenancy of the instance that you are modifying
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hosts
  /?Action=ModifyInstancePlacement:
    get:
      summary: Modify Instance Placement
      description: |-
        Set the instance affinity value for a specific stopped instance and modify the
                    instance tenancy setting.
      operationId: modifyinstanceplacement
      x-api-path-slug: actionmodifyinstanceplacement-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure idempotency
          of the request
        type: string
      - in: query
        name: CurrencyCode
        description: The currency in which the totalUpfrontPrice, LimitPrice,            and
          totalHourlyPrice amounts are specified
        type: string
      - in: query
        name: HostIdSet.N
        description: The ID/s of the Dedicated Host/s that the reservation will be
          associated            with
        type: string
      - in: query
        name: LimitPrice
        description: The specified limit is checked against the total upfront cost
          of the reservation            (calculated as the offerings upfront cost
          multiplied by the host count)
        type: string
      - in: query
        name: OfferingId
        description: The ID of the offering
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=ModifySnapshotAttribute:
    get:
      summary: Modify Snapshot Attribute
      description: Adds or removes permission settings for the specified snapshot.
      operationId: modifysnapshotattribute
      x-api-path-slug: actionmodifysnapshotattribute-get
      parameters:
      - in: query
        name: AutoEnableIO
        description: Indicates whether the volume should be auto-enabled for I/O operations
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshot
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