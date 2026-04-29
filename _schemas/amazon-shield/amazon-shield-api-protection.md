---
description: Protection schema from api
layout: schema
name: Protection
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: ResourceArn
  type: string
- description: ''
  name: HealthCheckIds
  type: array
- description: ''
  name: ProtectionArn
  type: string
provider_name: Amazon Shield
provider_slug: amazon-shield
schema_file: json-schema/amazon-shield-api-protection-schema.json
slug: amazon-shield-api-protection
source_filename: amazon-shield-api-protection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-protection-schema.json\",\n  \"title\": \"Protection\",\n  \"description\": \"Protection schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"ResourceArn\": {\n      \"type\": \"string\"\n    },\n    \"HealthCheckIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ProtectionArn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-protection-schema.json
tags:
- AWS
- DDoS Protection
- Networking
- Security
title: Protection
---
