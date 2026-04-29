---
description: ScanRequest schema from Palo Alto Networks Prisma AIRS API
layout: schema
name: ScanRequest
properties_list:
- description: Reference to the AI security profile to apply during scanning.
  name: ai_profile
  type: object
- description: Array of prompt/response pairs to scan. Each item represents one LLM interaction. For batch scanning, include multiple items.
  name: contents
  type: array
- description: Optional caller-supplied transaction ID for correlating scan requests with application-side records.
  name: tr_id
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-api-scan-request-schema.json
slug: prisma-airs-api-scan-request
source_filename: prisma-airs-api-scan-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanRequest\",\n  \"description\": \"ScanRequest schema from Palo Alto Networks Prisma AIRS API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-scan-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ai_profile\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"profile_name\"\n      ],\n      \"properties\": {\n        \"profile_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the AI security profile to use for this scan. The profile determines which detections are active and their sensitivity. Must reference an existing profile configured for the tenant.\"\n        }\n      },\n      \"description\": \"Reference to the AI security profile to apply during scanning.\"\n    },\n    \"contents\": {\n      \"type\": \"array\",\n      \"minItems\"\
  : 1,\n      \"description\": \"Array of prompt/response pairs to scan. Each item represents one LLM interaction. For batch scanning, include multiple items.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"prompt\": {\n            \"type\": \"string\",\n            \"description\": \"The user prompt or input text sent to the AI model. Evaluated for prompt injection, jailbreak attempts, and other input-side threats.\",\n            \"maxLength\": 32000\n          },\n          \"response\": {\n            \"type\": \"string\",\n            \"description\": \"The AI model response or output text. When provided, also evaluated for data leakage, toxic content, and other output-side threats. May be omitted to scan only the prompt.\",\n            \"maxLength\": 64000\n          }\n        }\n      }\n    },\n    \"tr_id\": {\n      \"type\": \"string\",\n      \"description\": \"Optional caller-supplied transaction ID for correlating scan requests\
  \ with application-side records.\"\n    }\n  },\n  \"required\": [\n    \"ai_profile\",\n    \"contents\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-scan-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ScanRequest
---
