---
description: CopyFileRequest schema from Backblaze B2 Native API
layout: schema
name: CopyFileRequest
properties_list:
- description: The ID of the file to copy
  name: sourceFileId
  type: string
- description: The name for the new file
  name: fileName
  type: string
- description: Bucket ID to copy to (defaults to source bucket)
  name: destinationBucketId
  type: string
- description: Byte range to copy
  name: range
  type: string
- description: Whether to copy or replace metadata
  name: metadataDirective
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-copy-file-request-schema.json
slug: b2-native-api-copy-file-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: CopyFileRequest
---
