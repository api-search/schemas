---
description: What the credentials allow
layout: schema
name: AllowedCapabilities
properties_list:
- description: A list of capabilities
  name: capabilities
  type: array
- description: Bucket ID restricted to, or null
  name: bucketId
  type: string
- description: Bucket name restricted to, or null
  name: bucketName
  type: string
- description: File name prefix restriction, or null
  name: namePrefix
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-allowed-capabilities-schema.json
slug: b2-native-api-allowed-capabilities
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: AllowedCapabilities
---
