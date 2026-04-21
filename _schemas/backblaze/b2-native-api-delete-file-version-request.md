---
description: DeleteFileVersionRequest schema from Backblaze B2 Native API
layout: schema
name: DeleteFileVersionRequest
properties_list:
- description: The name of the file
  name: fileName
  type: string
- description: The ID of the file version to delete
  name: fileId
  type: string
- description: Set to true to bypass object lock governance mode
  name: bypassGovernance
  type: boolean
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-delete-file-version-request-schema.json
slug: b2-native-api-delete-file-version-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: DeleteFileVersionRequest
---
