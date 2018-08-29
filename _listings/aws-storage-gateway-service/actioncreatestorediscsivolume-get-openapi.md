---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Create Stored SCSI Volume
  version: 1.0.0
  description: Creates a volume on a specified gateway.
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