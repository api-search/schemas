---
description: AIProfile schema from Palo Alto Networks Prisma AIRS API
layout: schema
name: AIProfile
properties_list:
- description: Unique identifier of the profile.
  name: profile_id
  type: string
- description: Profile name used to reference this profile in scan requests.
  name: profile_name
  type: string
- description: Human-readable description of the profile purpose and use case.
  name: description
  type: string
- description: Detection categories configured in this profile.
  name: detection_categories
  type: array
- description: Timestamp when the profile was created.
  name: created_at
  type: string
- description: Timestamp of the most recent profile modification.
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-api-ai-profile-schema.json
slug: prisma-airs-api-ai-profile
source_filename: prisma-airs-api-ai-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AIProfile\",\n  \"description\": \"AIProfile schema from Palo Alto Networks Prisma AIRS API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-ai-profile-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profile_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the profile.\"\n    },\n    \"profile_name\": {\n      \"type\": \"string\",\n      \"description\": \"Profile name used to reference this profile in scan requests.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the profile purpose and use case.\"\n    },\n    \"detection_categories\": {\n      \"type\": \"array\",\n      \"description\": \"Detection categories configured in this profile.\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"category\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"prompt_injection\",\n              \"jailbreak\",\n              \"data_leakage\",\n              \"toxic_content\",\n              \"malicious_url\",\n              \"pii_exposure\",\n              \"model_abuse\"\n            ]\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this detection category is active.\"\n          },\n          \"sensitivity\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"low\",\n              \"medium\",\n              \"high\"\n            ],\n            \"description\": \"Detection sensitivity threshold.\"\n          },\n          \"action\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"alert\",\n              \"block\",\n              \"log\"\n            ],\n            \"description\": \"\
  Enforcement action when this category triggers.\"\n          }\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the profile was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent profile modification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-ai-profile-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AIProfile
---
