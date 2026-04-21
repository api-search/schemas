---
description: A Backblaze B2 application key
layout: schema
name: ApplicationKey
properties_list:
- description: A name for this key
  name: keyName
  type: string
- description: The ID of the newly created key
  name: applicationKeyId
  type: string
- description: The secret key - only returned at creation time
  name: applicationKey
  type: string
- description: The account this key is associated with
  name: accountId
  type: string
- description: A list of capabilities this key has
  name: capabilities
  type: array
- description: When this key expires, or null for no expiration
  name: expirationTimestamp
  type: integer
- description: Restrict key to this bucket, or null for all buckets
  name: bucketId
  type: string
- description: Restrict key to file names starting with this prefix
  name: namePrefix
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-application-key-schema.json
slug: b2-native-api-application-key
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ApplicationKey
---
