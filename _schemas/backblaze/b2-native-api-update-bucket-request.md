---
description: UpdateBucketRequest schema from Backblaze B2 Native API
layout: schema
name: UpdateBucketRequest
properties_list:
- description: The account ID
  name: accountId
  type: string
- description: The ID of the bucket to update
  name: bucketId
  type: string
- description: New privacy setting
  name: bucketType
  type: string
- description: New bucket info
  name: bucketInfo
  type: object
- description: New CORS rules
  name: corsRules
  type: array
- description: New lifecycle rules
  name: lifecycleRules
  type: array
- description: Only update if bucket revision matches this value
  name: ifRevisionIs
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-update-bucket-request-schema.json
slug: b2-native-api-update-bucket-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: UpdateBucketRequest
---
