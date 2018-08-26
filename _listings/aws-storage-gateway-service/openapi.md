---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddCache:
    get:
      summary: Add Cache
      description: Configures one or more gateway local disks as cache for a cached-volume
        gateway.
      operationId: addCache
      x-api-path-slug: actionaddcache-get
      parameters:
      - in: query
        name: DiskIds
        description: 'Type: array of Strings'
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache
  /?Action=DescribeCache:
    get:
      summary: Describe Cache
      description: Returns information about the cache of a gateway.
      operationId: describeCache
      x-api-path-slug: actiondescribecache-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache
  /?Action=ResetCache:
    get:
      summary: Reset Cache
      description: |-
        Resets all cache disks that have encountered a error and makes the disks available
                 for reconfiguration as cache storage.
      operationId: resetCache
      x-api-path-slug: actionresetcache-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache
  /?Action=CreateCachediSCSIVolume:
    get:
      summary: Create Cached SCSI Volume
      description: Creates a cached volume on a specified cached gateway.
      operationId: createCachediSCSIVolume
      x-api-path-slug: actioncreatecachediscsivolume-get
      parameters:
      - in: query
        name: ClientToken
        description: 'Type: String'
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: NetworkInterfaceId
        description: 'Type: String'
        type: string
      - in: query
        name: SnapshotId
        description: 'Type: String'
        type: string
      - in: query
        name: SourceVolumeARN
        description: The ARN for an existing volume
        type: string
      - in: query
        name: TargetName
        description: 'Type: String'
        type: string
      - in: query
        name: VolumeSizeInBytes
        description: 'Type: Long'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cached SCSI Volume
  /?Action=DescribeCachediSCSIVolumes:
    get:
      summary: Describe Cached SCSI Volumes
      description: Returns a description of the gateway volumes specified in the request.
      operationId: describeCachediSCSIVolumes
      x-api-path-slug: actiondescribecachediscsivolumes-get
      parameters:
      - in: query
        name: VolumeARNs
        description: 'Type: array of Strings'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cached SCSI Volumes
---