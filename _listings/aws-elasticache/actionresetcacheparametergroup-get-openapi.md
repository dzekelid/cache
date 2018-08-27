---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API Reset Cache Parameter Group
  version: 1.0.0
  description: |-
    Modifies the parameters of a cache
                parameter group to the engine or system default value.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AuthorizeCacheSecurityGroupIngress:
    get:
      summary: Authorize Cache Security Group Ingress
      description: |-
        Allows network ingress to a cache
                    security group.
      operationId: authorizeCacheSecurityGroupIngress
      x-api-path-slug: actionauthorizecachesecuritygroupingress-get
      parameters:
      - in: query
        name: CacheSecurityGroupName
        description: The cache security group that allows network ingress
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The Amazon EC2 security group to be authorized for ingress to
          the cache security group
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the Amazon EC2 security group owner
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Security Groups
  /?Action=CreateCacheCluster:
    get:
      summary: Create Cache Cluster
      description: Creates a cache cluster.
      operationId: createCacheCluster
      x-api-path-slug: actioncreatecachecluster-get
      parameters:
      - in: query
        name: AuthToken
        description: Reserved parameter
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: This parameter is currently disabled
        type: string
      - in: query
        name: AZMode
        description: Specifies whether the nodes in this Memcached cluster are created
          in a single Availability Zone or             created across multiple Availability
          Zones in the clusters region
        type: string
      - in: query
        name: CacheClusterId
        description: The node group (shard) identifier
        type: string
      - in: query
        name: CacheNodeType
        description: The compute and memory capacity of the nodes in the node group
          (shard)
        type: string
      - in: query
        name: CacheParameterGroupName
        description: The name of the parameter group to associate with this cache
          cluster
        type: string
      - in: query
        name: CacheSecurityGroupNames.CacheSecurityGroupName.N
        description: A list of security group names to associate with this cache cluster
        type: string
      - in: query
        name: CacheSubnetGroupName
        description: The name of the subnet group to be used for the cache cluster
        type: string
      - in: query
        name: Engine
        description: The name of the cache engine to be used for this cache cluster
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the cache engine to be used for this cache
          cluster
        type: string
      - in: query
        name: NotificationTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon Simple Notification
          Service (SNS) topic           to which notifications are sent
        type: string
      - in: query
        name: NumCacheNodes
        description: The initial number of cache nodes that the cache cluster has
        type: string
      - in: query
        name: Port
        description: The port number on which each of the cache nodes  accepts connections
        type: string
      - in: query
        name: PreferredAvailabilityZone
        description: The EC2 Availability Zone in which the cache cluster is created
        type: string
      - in: query
        name: PreferredAvailabilityZones.PreferredAvailabilityZone.N
        description: A list of the Availability Zones in which cache nodes are created
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: Specifies the weekly time range during which maintenance            on
          the cache cluster is performed
        type: string
      - in: query
        name: ReplicationGroupId
        description: Important
        type: string
      - in: query
        name: SecurityGroupIds.SecurityGroupId.N
        description: One or more VPC security groups associated with the cache cluster
        type: string
      - in: query
        name: SnapshotArns.SnapshotArn.N
        description: A single-element string list containing an Amazon Resource Name
          (ARN) that uniquely identifies a Redis RDB snapshot file stored in Amazon
          S3
        type: string
      - in: query
        name: SnapshotName
        description: The name of a Redis snapshot from which to restore data into
          the new node group (shard)
        type: string
      - in: query
        name: SnapshotRetentionLimit
        description: The number of days for which ElastiCache retains automatic snapshots
          before deleting them
        type: string
      - in: query
        name: SnapshotWindow
        description: The daily time range (in UTC) during which ElastiCache begins
          taking a daily snapshot of your node group (shard)
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of cost allocation tags to be added to this resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Clusters
  /?Action=CreateCacheParameterGroup:
    get:
      summary: Create Cache Parameter Group
      description: Creates a new cache parameter group.
      operationId: createCacheParameterGroup
      x-api-path-slug: actioncreatecacheparametergroup-get
      parameters:
      - in: query
        name: CacheParameterGroupFamily
        description: The name of the cache parameter group family that the cache parameter
          group can be used with
        type: string
      - in: query
        name: CacheParameterGroupName
        description: A user-specified name for the cache parameter group
        type: string
      - in: query
        name: Description
        description: A user-specified description for the cache parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameter Groups
  /?Action=CreateCacheSecurityGroup:
    get:
      summary: Create Cache Security Group
      description: Creates a new cache security group.
      operationId: createCacheSecurityGroup
      x-api-path-slug: actioncreatecachesecuritygroup-get
      parameters:
      - in: query
        name: CacheSecurityGroupName
        description: A name for the cache security group
        type: string
      - in: query
        name: Description
        description: A description for the cache security group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Security Groups
  /?Action=CreateCacheSubnetGroup:
    get:
      summary: Create Cache Subnet Group
      description: Creates a new cache subnet group.
      operationId: createCacheSubnetGroup
      x-api-path-slug: actioncreatecachesubnetgroup-get
      parameters:
      - in: query
        name: CacheSubnetGroupDescription
        description: A description for the cache subnet group
        type: string
      - in: query
        name: CacheSubnetGroupName
        description: A name for the cache subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: A list of VPC subnet IDs for the cache subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups
  /?Action=DeleteCacheCluster:
    get:
      summary: Delete Cache Cluster
      description: Deletes a previously provisioned cache cluster.
      operationId: deleteCacheCluster
      x-api-path-slug: actiondeletecachecluster-get
      parameters:
      - in: query
        name: CacheClusterId
        description: The cache cluster identifier for the cluster to be deleted
        type: string
      - in: query
        name: FinalSnapshotIdentifier
        description: The user-supplied name of a final cache cluster snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Clusters
  /?Action=DeleteCacheParameterGroup:
    get:
      summary: Delete Cache Parameter Group
      description: |-
        Deletes the specified cache parameter
                    group.
      operationId: deleteCacheParameterGroup
      x-api-path-slug: actiondeletecacheparametergroup-get
      parameters:
      - in: query
        name: CacheParameterGroupName
        description: The name of the cache parameter group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameter Groups
  /?Action=DeleteCacheSecurityGroup:
    get:
      summary: Delete Cache Security Group
      description: Deletes a cache security group.
      operationId: deleteCacheSecurityGroup
      x-api-path-slug: actiondeletecachesecuritygroup-get
      parameters:
      - in: query
        name: CacheSecurityGroupName
        description: The name of the cache security group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Security Groups
  /?Action=DeleteCacheSubnetGroup:
    get:
      summary: Delete Cache Subnet Group
      description: Deletes a cache subnet group.
      operationId: deleteCacheSubnetGroup
      x-api-path-slug: actiondeletecachesubnetgroup-get
      parameters:
      - in: query
        name: CacheSubnetGroupName
        description: The name of the cache subnet group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups
  /?Action=DescribeCacheClusters:
    get:
      summary: Describe Cache Clusters
      description: |-
        Returns information about all provisioned
                    cache clusters if no cache cluster identifier is specified, or about a specific cache
                    cluster if a cache cluster identifier is supplied.
      operationId: describeCacheClusters
      x-api-path-slug: actiondescribecacheclusters-get
      parameters:
      - in: query
        name: CacheClusterId
        description: The user-supplied cluster identifier
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: ShowCacheNodeInfo
        description: An optional flag that can be included in the DescribeCacheCluster
          request             to retrieve information about the individual cache nodes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Clusters
  /?Action=DescribeCacheEngineVersions:
    get:
      summary: Describe Cache Engine Versions
      description: |-
        Returns a list of the available cache
                    engines and their versions.
      operationId: describeCacheEngineVersions
      x-api-path-slug: actiondescribecacheengineversions-get
      parameters:
      - in: query
        name: CacheParameterGroupFamily
        description: The name of a specific cache parameter group family to return
          details for
        type: string
      - in: query
        name: DefaultOnly
        description: If true, specifies that only the default version of the specified
          engine or engine            and major version combination is to be returned
        type: string
      - in: query
        name: Engine
        description: The cache engine to return
        type: string
      - in: query
        name: EngineVersion
        description: The cache engine version to return
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Engine Versions
  /?Action=DescribeCacheParameterGroups:
    get:
      summary: Describe Cache Parameter Groups
      description: |-
        Returns a list of cache parameter group
                    descriptions.
      operationId: describeCacheParameterGroups
      x-api-path-slug: actiondescribecacheparametergroups-get
      parameters:
      - in: query
        name: CacheParameterGroupName
        description: The name of a specific cache parameter group to return details
          for
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameter Groups
  /?Action=DescribeCacheParameters:
    get:
      summary: Describe Cache Parameters
      description: |-
        Returns the detailed parameter list for a
                    particular cache parameter group.
      operationId: describeCacheParameters
      x-api-path-slug: actiondescribecacheparameters-get
      parameters:
      - in: query
        name: CacheParameterGroupName
        description: The name of a specific cache parameter group to return details
          for
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: Source
        description: The parameter types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameters
  /?Action=DescribeCacheSecurityGroups:
    get:
      summary: Describe Cache Security Groups
      description: |-
        Returns a list of cache security group
                    descriptions.
      operationId: describeCacheSecurityGroups
      x-api-path-slug: actiondescribecachesecuritygroups-get
      parameters:
      - in: query
        name: CacheSecurityGroupName
        description: The name of the cache security group to return details for
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Security Groups
  /?Action=DescribeCacheSubnetGroups:
    get:
      summary: Describe Cache Subnet Groups
      description: |-
        Returns a list of cache subnet group
                    descriptions.
      operationId: describeCacheSubnetGroups
      x-api-path-slug: actiondescribecachesubnetgroups-get
      parameters:
      - in: query
        name: CacheSubnetGroupName
        description: The name of the cache subnet group to return details for
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups
  /?Action=DescribeReservedCacheNodes:
    get:
      summary: Describe Reserved Cache Nodes
      description: |-
        Returns information about reserved cache
                    nodes for this account, or about a specified reserved cache node.
      operationId: describeReservedCacheNodes
      x-api-path-slug: actiondescribereservedcachenodes-get
      parameters:
      - in: query
        name: CacheNodeType
        description: The cache node type filter value
        type: string
      - in: query
        name: Duration
        description: The duration filter value, specified in years or seconds
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: OfferingType
        description: The offering type filter value
        type: string
      - in: query
        name: ProductDescription
        description: The product description filter value
        type: string
      - in: query
        name: ReservedCacheNodeId
        description: The reserved cache node identifier filter value
        type: string
      - in: query
        name: ReservedCacheNodesOfferingId
        description: The offering identifier filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Cache Nodes
  /?Action=DescribeReservedCacheNodesOfferings:
    get:
      summary: Describe Reserved Cache Nodes Offerings
      description: |-
        Lists available reserved cache
                    node offerings.
      operationId: describeReservedCacheNodesOfferings
      x-api-path-slug: actiondescribereservedcachenodesofferings-get
      parameters:
      - in: query
        name: CacheNodeType
        description: The cache node type filter value
        type: string
      - in: query
        name: Duration
        description: Duration filter value, specified in years or seconds
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: OfferingType
        description: The offering type filter value
        type: string
      - in: query
        name: ProductDescription
        description: The product description filter value
        type: string
      - in: query
        name: ReservedCacheNodesOfferingId
        description: The offering identifier filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Cache Nodes
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
  /?Action=PurchaseReservedCacheNodesOffering:
    get:
      summary: Purchase Reserved Cache Nodes Offering
      description: |-
        Allows you to purchase a reserved
                    cache node offering.
      operationId: purchaseReservedCacheNodesOffering
      x-api-path-slug: actionpurchasereservedcachenodesoffering-get
      parameters:
      - in: query
        name: CacheNodeCount
        description: The number of cache node instances to reserve
        type: string
      - in: query
        name: ReservedCacheNodeId
        description: A customer-specified identifier to track this reservation
        type: string
      - in: query
        name: ReservedCacheNodesOfferingId
        description: The ID of the reserved cache node offering to purchase
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Cache Nodes
  /?Action=RebootCacheCluster:
    get:
      summary: Reboot Cache Cluster
      description: |-
        Reboots some, or all, of the cache nodes
                    within a provisioned cache cluster.
      operationId: rebootCacheCluster
      x-api-path-slug: actionrebootcachecluster-get
      parameters:
      - in: query
        name: CacheClusterId
        description: The cache cluster identifier
        type: string
      - in: query
        name: CacheNodeIdsToReboot.CacheNodeId.N
        description: A list of cache node IDs to reboot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Clusters
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