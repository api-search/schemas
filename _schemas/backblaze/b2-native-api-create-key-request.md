---
description: CreateKeyRequest schema from Backblaze B2 Native API
layout: schema
name: CreateKeyRequest
properties_list:
- description: ''
  name: accountId
  type: string
- description: List of capabilities for the key
  name: capabilities
  type: array
- description: A name for the key (letters, numbers, hyphens)
  name: keyName
  type: string
- description: Duration before key expires
  name: validDurationInSeconds
  type: integer
- description: Restrict key to this bucket
  name: bucketId
  type: string
- description: Restrict key to files with this prefix
  name: namePrefix
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-create-key-request-schema.json
slug: b2-native-api-create-key-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: CreateKeyRequest
---
