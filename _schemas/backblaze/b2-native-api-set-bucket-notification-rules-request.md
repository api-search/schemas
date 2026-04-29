---
description: SetBucketNotificationRulesRequest schema from Backblaze B2 Native API
layout: schema
name: SetBucketNotificationRulesRequest
properties_list:
- description: ''
  name: bucketId
  type: string
- description: ''
  name: rules
  type: array
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-set-bucket-notification-rules-request-schema.json
slug: b2-native-api-set-bucket-notification-rules-request
source_filename: b2-native-api-set-bucket-notification-rules-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-set-bucket-notification-rules-request-schema.json\",\n  \"title\": \"SetBucketNotificationRulesRequest\",\n  \"description\": \"SetBucketNotificationRulesRequest schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"example\": \"e73ede9969c64355ef8b\"\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/NotificationRule\"\n      }\n    }\n  },\n  \"required\": [\n    \"bucketId\",\n    \"rules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-set-bucket-notification-rules-request-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: SetBucketNotificationRulesRequest
---
