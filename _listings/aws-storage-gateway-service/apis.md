---
name: AWS Storage Gateway Service
x-slug: aws-storage-gateway-service
description: The AWS Storage Gateway service seamlessly enables hybrid storage between
  on-premises storage environments andthe AWS Cloud. It combines a multi-protocol
  storage appliance with highly efficient network connectivity toAmazon cloud storageservices,
  delivering local performance with virtually unlimited scale. Customers use it in
  remote offices and datacenters for hybrid cloud workloads, backup and restore, archive,
  disaster recovery, and tiered storage.The Storage Gateway virtual appliance connects
  seamlessly to your local infrastructure as a file server, as a volume, or as a virtual
  tape library (VTL). This seamless connection makes it simple for organizations to
  augment existing on-premises storage investments with the high scalability, extreme
  durability and low cost of cloud storage.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Volume
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Storage Gateway Service API - Create Cached SCSI Volume
  x-api-slug: actioncreatecachediscsivolume-get
  description: Creates a cached volume on a specified cached gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actioncreatecachediscsivolume-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actioncreatecachediscsivolume-get-openapi.md
- name: AWS Storage Gateway Service API - Create Snapshot From Volume Recovery Point
  x-api-slug: actioncreatesnapshotfromvolumerecoverypoint-get
  description: Initiates a snapshot of a gateway from a volume recovery point.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actioncreatesnapshotfromvolumerecoverypoint-get-openapi.md
- name: AWS Storage Gateway Service API - Create Stored SCSI Volume
  x-api-slug: actioncreatestorediscsivolume-get
  description: Creates a volume on a specified gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actioncreatestorediscsivolume-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actioncreatestorediscsivolume-get-openapi.md
- name: AWS Storage Gateway Service API - Delete Volume
  x-api-slug: actiondeletevolume-get
  description: Deletes the specified gateway volume that you previously created using
    the.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actiondeletevolume-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Cached SCSI Volumes
  x-api-slug: actiondescribecachediscsivolumes-get
  description: Returns a description of the gateway volumes specified in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actiondescribecachediscsivolumes-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Stored SCSI Volumes
  x-api-slug: actiondescribestorediscsivolumes-get
  description: Returns the description of the gateway volumes specified in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actiondescribestorediscsivolumes-get-openapi.md
- name: AWS Storage Gateway Service API - List Volume Initiators
  x-api-slug: actionlistvolumeinitiators-get
  description: Lists iSCSI initiators that are connected to a volume.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actionlistvolumeinitiators-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actionlistvolumeinitiators-get-openapi.md
- name: AWS Storage Gateway Service API - List Volume Recovery Points
  x-api-slug: actionlistvolumerecoverypoints-get
  description: Lists the recovery points for a specified gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actionlistvolumerecoverypoints-get-openapi.md
- name: AWS Storage Gateway Service API - List Volumes
  x-api-slug: actionlistvolumes-get
  description: Lists the iSCSI stored volumes of a gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actionlistvolumes-get-openapi.md
- name: AWS Storage Gateway Service API - Delete Volume
  x-api-slug: actiondeletevolume-get
  description: Deletes the specified gateway volume that you previously created using
    the.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actiondeletevolume-get-openapi.md
- name: AWS Storage Gateway Service API - List Volumes
  x-api-slug: actionlistvolumes-get
  description: Lists the iSCSI stored volumes of a gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actionlistvolumes-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Cached SCSI Volumes
  x-api-slug: actiondescribecachediscsivolumes-get
  description: Returns a description of the gateway volumes specified in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actiondescribecachediscsivolumes-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Stored SCSI Volumes
  x-api-slug: actiondescribestorediscsivolumes-get
  description: Returns the description of the gateway volumes specified in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actiondescribestorediscsivolumes-get-openapi.md
- name: AWS Storage Gateway Service API - Delete Volume
  x-api-slug: actiondeletevolume-get
  description: Deletes the specified gateway volume that you previously created using
    the.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actiondeletevolume-get-openapi.md
- name: AWS Storage Gateway Service API - List Volumes
  x-api-slug: actionlistvolumes-get
  description: Lists the iSCSI stored volumes of a gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/volume/master/_listings/aws-storage-gateway-service/actionlistvolumes-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.step.functions.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.storage.gateway.service.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/storagegateway/latest/APIReference
- type: x-faq
  url: https://aws.amazon.com/storagegateway/faqs/
- type: x-pricing
  url: https://aws.amazon.com/storagegateway/pricing/
- type: x-website
  url: https://aws.amazon.com/storagegateway/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---