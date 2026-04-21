---
description: ListKeysRequest schema from Backblaze B2 Native API
layout: schema
name: ListKeysRequest
properties_list:
- description: ''
  name: accountId
  type: string
- description: Maximum number of keys to return
  name: maxKeyCount
  type: integer
- description: Start listing from this key ID
  name: startApplicationKeyId
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-list-keys-request-schema.json
slug: b2-native-api-list-keys-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ListKeysRequest
---
