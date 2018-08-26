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
tags: Cache
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/cache/master/_listings/aws-storage-gateway-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Storage Gateway Service API - Add Cache
  x-api-slug: actionaddcache-get
  description: Configures one or more gateway local disks as cache for a cached-volume
    gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cache/master/_listings/aws-storage-gateway-service/actionaddcache-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cache/master/_listings/aws-storage-gateway-service/actionaddcache-get-openapi.md
- name: AWS Storage Gateway Service API - Describe Cache
  x-api-slug: actiondescribecache-get
  description: Returns information about the cache of a gateway.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cache/master/_listings/aws-storage-gateway-service/actiondescribecache-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cache/master/_listings/aws-storage-gateway-service/actiondescribecache-get-openapi.md
- name: AWS Storage Gateway Service API - Reset Cache
  x-api-slug: actionresetcache-get
  description: |-
    Resets all cache disks that have encountered a error and makes the disks available
             for reconfiguration as cache storage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AWSStorageGateway.png
  humanURL: https://aws.amazon.com/storagegateway/
  baseURL: :///
  tags: Amazon Web Services, Gateway, Data, Stack Network, API Service Provider, API
    Service Provider, API Provider, Databases, Deployments, Profiles, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cache/master/_listings/aws-storage-gateway-service/actionresetcache-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cache/master/_listings/aws-storage-gateway-service/actionresetcache-get-openapi.md
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
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cache/master/_listings/aws-storage-gateway-service/actioncreatecachediscsivolume-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cache/master/_listings/aws-storage-gateway-service/actioncreatecachediscsivolume-get-openapi.md
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