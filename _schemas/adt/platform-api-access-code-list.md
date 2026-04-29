---
description: List of access codes.
layout: schema
name: AccessCodeList
properties_list:
- description: Array of access codes.
  name: accessCodes
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-access-code-list-schema.json
slug: platform-api-access-code-list
source_filename: platform-api-access-code-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-access-code-list-schema.json\",\n  \"title\": \"AccessCodeList\",\n  \"description\": \"List of access codes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessCodes\": {\n      \"type\": \"array\",\n      \"description\": \"Array of access codes.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An access code for a security system.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier of the access code.\",\n            \"example\": \"code-001\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name for the access code.\",\n            \"example\": \"Master Code\"\n          },\n          \"type\": {\n            \"\
  type\": \"string\",\n            \"description\": \"Type of access code.\",\n            \"enum\": [\n              \"master\",\n              \"standard\",\n              \"temporary\",\n              \"duress\"\n            ],\n            \"example\": \"standard\"\n          },\n          \"expiresAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Expiration timestamp for temporary codes.\",\n            \"example\": \"2025-03-20T23:59:59Z\"\n          },\n          \"permissions\": {\n            \"type\": \"array\",\n            \"description\": \"List of permissions granted by this code.\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-access-code-list-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: AccessCodeList
---
