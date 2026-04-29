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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-application-key-schema.json\",\n  \"title\": \"ApplicationKey\",\n  \"description\": \"A Backblaze B2 application key\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyName\": {\n      \"type\": \"string\",\n      \"description\": \"A name for this key\",\n      \"example\": \"my-app-key\"\n    },\n    \"applicationKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the newly created key\",\n      \"example\": \"0014a98f9d9e8d0000000001\"\n    },\n    \"applicationKey\": {\n      \"type\": \"string\",\n      \"description\": \"The secret key - only returned at creation time\",\n      \"example\": \"K0014a98f9d9e8d0000000001a9b2c3d4\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account this key is associated with\",\n\
  \      \"example\": \"abc123def456\"\n    },\n    \"capabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of capabilities this key has\"\n    },\n    \"expirationTimestamp\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"When this key expires, or null for no expiration\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Restrict key to this bucket, or null for all buckets\"\n    },\n    \"namePrefix\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Restrict key to file names starting with this prefix\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-application-key-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: ApplicationKey
---
