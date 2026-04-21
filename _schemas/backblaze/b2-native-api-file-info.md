---
description: Information about a stored file
layout: schema
name: FileInfo
properties_list:
- description: The unique identifier for this version of this file
  name: fileId
  type: string
- description: The name of the file
  name: fileName
  type: string
- description: The account that owns the file
  name: accountId
  type: string
- description: The bucket that the file is in
  name: bucketId
  type: string
- description: The size of the file in bytes
  name: contentLength
  type: integer
- description: The SHA1 checksum of the bytes in the file
  name: contentSha1
  type: string
- description: The MIME type of the file
  name: contentType
  type: string
- description: Custom information about the file
  name: fileInfo
  type: object
- description: The action that created this file version
  name: action
  type: string
- description: Milliseconds since midnight, January 1, 1970 UTC
  name: uploadTimestamp
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-file-info-schema.json
slug: b2-native-api-file-info
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: FileInfo
---
