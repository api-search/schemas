---
description: ListFileNamesRequest schema from Backblaze B2 Native API
layout: schema
name: ListFileNamesRequest
properties_list:
- description: The bucket to list
  name: bucketId
  type: string
- description: Start listing from this file name
  name: startFileName
  type: string
- description: Maximum number of files to return (1-10000)
  name: maxFileCount
  type: integer
- description: Prefix to filter file names
  name: prefix
  type: string
- description: Delimiter used for virtual folder simulation
  name: delimiter
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-file-names-request-schema.json
slug: b2-native-api-list-file-names-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListFileNamesRequest
---
