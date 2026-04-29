---
description: Error schema from Bandwidth messaging API
layout: schema
name: Error
properties_list:
- description: The error type identifier
  name: type
  type: string
- description: A human-readable description of the error
  name: description
  type: string
- description: ''
  name: fieldErrors
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-error-schema.json
slug: messaging-error
source_filename: messaging-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Error schema from Bandwidth messaging API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The error type identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error\"\n    },\n    \"fieldErrors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"description\": \"The field that caused the error\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Description of the field error\"\n      \
  \    }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-error-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Error
---
