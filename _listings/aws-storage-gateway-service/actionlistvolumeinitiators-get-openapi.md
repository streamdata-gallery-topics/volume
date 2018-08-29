---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API List Volume Initiators
  version: 1.0.0
  description: Lists iSCSI initiators that are connected to a volume.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
  /?Action=CreateSnapshotFromVolumeRecoveryPoint:
    get:
      summary: Create Snapshot From Volume Recovery Point
      description: Initiates a snapshot of a gateway from a volume recovery point.
      operationId: createSnapshotFromVolumeRecoveryPoint
      x-api-path-slug: actioncreatesnapshotfromvolumerecoverypoint-get
      parameters:
      - in: query
        name: SnapshotDescription
        description: 'Type: String'
        type: string
      - in: query
        name: VolumeARN
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateStorediSCSIVolume:
    get:
      summary: Create Stored SCSI Volume
      description: Creates a volume on a specified gateway.
      operationId: createStorediSCSIVolume
      x-api-path-slug: actioncreatestorediscsivolume-get
      parameters:
      - in: query
        name: DiskId
        description: The unique identifier for the gateway local disk that is configured
          as a stored         volume
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The network interface of the gateway on which to expose the iSCSI
          target
        type: string
      - in: query
        name: PreserveExistingData
        description: Specify this field as true if you want to preserve the data on
          the local disk
        type: string
      - in: query
        name: SnapshotId
        description: The snapshot ID (e
        type: string
      - in: query
        name: TargetName
        description: The name of the iSCSI target used by initiators to connect to
          the target and as a         suffix for the target ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stored SCSI Volume
  /?Action=DeleteVolume:
    get:
      summary: Delete Volume
      description: Deletes the specified gateway volume that you previously created
        using the.
      operationId: deleteVolume
      x-api-path-slug: actiondeletevolume-get
      parameters:
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volumes
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
  /?Action=DescribeStorediSCSIVolumes:
    get:
      summary: Describe Stored SCSI Volumes
      description: Returns the description of the gateway volumes specified in the
        request.
      operationId: describeStorediSCSIVolumes
      x-api-path-slug: actiondescribestorediscsivolumes-get
      parameters:
      - in: query
        name: VolumeARNs
        description: An array of strings where each string represents the Amazon Resource
          Name (ARN) of a         stored volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stored SCSI Volumes
  /?Action=ListVolumeInitiators:
    get:
      summary: List Volume Initiators
      description: Lists iSCSI initiators that are connected to a volume.
      operationId: listVolumeInitiators
      x-api-path-slug: actionlistvolumeinitiators-get
      parameters:
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volume Initiators
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