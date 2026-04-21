---
description: CreateBucketRequest schema from Backblaze B2 Native API
layout: schema
name: CreateBucketRequest
properties_list:
- description: The account ID
  name: accountId
  type: string
- description: The name of the new bucket
  name: bucketName
  type: string
- description: Privacy setting for the bucket
  name: bucketType
  type: string
- description: User-defined info to store with the bucket
  name: bucketInfo
  type: object
- description: CORS rules for the bucket
  name: corsRules
  type: array
- description: Lifecycle rules for the bucket
  name: lifecycleRules
  type: array
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-create-bucket-request-schema.json
slug: b2-native-api-create-bucket-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: CreateBucketRequest
---
