---
description: Specifies the inventory configuration for an Amazon S3 bucket. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketGETInventoryConfig.html">GET Bucket inventory</a> in the <i>Amazon S3 API Reference</i>.
layout: schema
name: InventoryConfiguration
properties_list:
- description: ''
  name: Destination
  type: object
- description: ''
  name: IsEnabled
  type: object
- description: ''
  name: Filter
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: IncludedObjectVersions
  type: object
- description: ''
  name: OptionalFields
  type: object
- description: ''
  name: Schedule
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-inventoryconfiguration-schema.json
slug: s3-inventoryconfiguration
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: InventoryConfiguration
---
