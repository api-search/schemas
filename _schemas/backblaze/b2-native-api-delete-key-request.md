---
description: DeleteKeyRequest schema from Backblaze B2 Native API
layout: schema
name: DeleteKeyRequest
properties_list:
- description: The ID of the key to delete
  name: applicationKeyId
  type: string
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-delete-key-request-schema.json
slug: b2-native-api-delete-key-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-delete-key-request-schema.json\",\n  \"title\": \"DeleteKeyRequest\",\n  \"description\": \"DeleteKeyRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the key to delete\",\n      \"example\": \"0014a98f9d9e8d0000000001\"\n    }\n  },\n  \"required\": [\n    \"applicationKeyId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-delete-key-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: DeleteKeyRequest
---
