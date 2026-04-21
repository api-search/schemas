---
description: Describes an Amazon S3 location that will receive the results of the restore request.
layout: schema
name: S3Location
properties_list:
- description: ''
  name: BucketName
  type: object
- description: ''
  name: Prefix
  type: object
- description: Contains the type of server-side encryption used.
  name: Encryption
  type: object
- description: ''
  name: CannedACL
  type: object
- description: ''
  name: AccessControlList
  type: object
- description: ''
  name: Tagging
  type: object
- description: ''
  name: UserMetadata
  type: object
- description: ''
  name: StorageClass
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-s3location-schema.json
slug: s3-s3location
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: S3Location
---
