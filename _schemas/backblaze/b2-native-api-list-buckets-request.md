---
description: ListBucketsRequest schema from Backblaze B2 Native API
layout: schema
name: ListBucketsRequest
properties_list:
- description: The account ID
  name: accountId
  type: string
- description: Filter to a specific bucket
  name: bucketId
  type: string
- description: Filter by bucket name
  name: bucketName
  type: string
- description: Filter by bucket type
  name: bucketTypes
  type: array
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-buckets-request-schema.json
slug: b2-native-api-list-buckets-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListBucketsRequest
---
