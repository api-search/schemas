---
description: FinishLargeFileRequest schema from Backblaze B2 Native API
layout: schema
name: FinishLargeFileRequest
properties_list:
- description: The file ID from b2_start_large_file
  name: fileId
  type: string
- description: SHA1 checksums of each part in order
  name: partSha1Array
  type: array
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-finish-large-file-request-schema.json
slug: b2-native-api-finish-large-file-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: FinishLargeFileRequest
---
