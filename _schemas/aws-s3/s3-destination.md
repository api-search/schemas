---
description: Specifies information about where to publish analysis or configuration results for an Amazon S3 bucket and S3 Replication Time Control (S3 RTC).
layout: schema
name: Destination
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Account
  type: object
- description: ''
  name: StorageClass
  type: object
- description: ''
  name: AccessControlTranslation
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
- description: ''
  name: ReplicationTime
  type: object
- description: ''
  name: Metrics
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-destination-schema.json
slug: s3-destination
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Destination
---
