---
description: AttackDetail schema from api
layout: schema
name: AttackDetail
properties_list:
- description: ''
  name: AttackId
  type: string
- description: ''
  name: ResourceArn
  type: string
- description: ''
  name: StartTime
  type: string
- description: ''
  name: EndTime
  type: string
- description: ''
  name: AttackCounters
  type: array
- description: ''
  name: Mitigations
  type: array
provider_name: Amazon Shield
provider_slug: amazon-shield
schema_file: json-schema/amazon-shield-api-attack-detail-schema.json
slug: amazon-shield-api-attack-detail
source_filename: amazon-shield-api-attack-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-attack-detail-schema.json\",\n  \"title\": \"AttackDetail\",\n  \"description\": \"AttackDetail schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttackId\": {\n      \"type\": \"string\"\n    },\n    \"ResourceArn\": {\n      \"type\": \"string\"\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"AttackCounters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SummarizedCounter\"\n      }\n    },\n    \"Mitigations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Mitigation\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-attack-detail-schema.json
tags:
- AWS
- DDoS Protection
- Networking
- Security
title: AttackDetail
---
