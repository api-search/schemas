---
description: Represents a B2 bucket
layout: schema
name: Bucket
properties_list:
- description: The account that owns the bucket
  name: accountId
  type: string
- description: The unique ID of the bucket
  name: bucketId
  type: string
- description: The unique name of the bucket
  name: bucketName
  type: string
- description: The bucket privacy setting
  name: bucketType
  type: string
- description: User-defined information stored with the bucket
  name: bucketInfo
  type: object
- description: CORS rules for the bucket
  name: corsRules
  type: array
- description: Lifecycle rules for the bucket
  name: lifecycleRules
  type: array
- description: The number of times the bucket info has been modified
  name: revision
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-bucket-schema.json
slug: b2-native-api-bucket
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: Bucket
---
