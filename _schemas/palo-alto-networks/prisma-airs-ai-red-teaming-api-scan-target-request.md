---
description: ScanTargetRequest schema from Palo Alto Networks Prisma AIRS AI Red Teaming API
layout: schema
name: ScanTargetRequest
properties_list:
- description: Display name for the scan target.
  name: name
  type: string
- description: Optional description of the target application.
  name: description
  type: string
- description: AI interface type of the target endpoint.
  name: type
  type: string
- description: URL of the AI application endpoint to scan.
  name: endpoint_url
  type: string
- description: AI model name to include in requests (e.g., gpt-4o, claude-3-5-sonnet-20241022).
  name: model
  type: string
- description: Authentication configuration for the target endpoint.
  name: auth_config
  type: object
- description: System prompt to include in requests to the target. Used to scope red teaming attacks to the intended application context.
  name: system_prompt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-ai-red-teaming-api-scan-target-request-schema.json
slug: prisma-airs-ai-red-teaming-api-scan-target-request
source_filename: prisma-airs-ai-red-teaming-api-scan-target-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanTargetRequest\",\n  \"description\": \"ScanTargetRequest schema from Palo Alto Networks Prisma AIRS AI Red Teaming API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-target-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the scan target.\",\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the target application.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"openai_chat\",\n        \"anthropic_messages\",\n        \"custom_http\",\n        \"huggingface\"\n      ],\n      \"description\": \"AI interface type of the target endpoint.\"\n    },\n    \"endpoint_url\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the AI application endpoint to scan.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"AI model name to include in requests (e.g., gpt-4o, claude-3-5-sonnet-20241022).\"\n    },\n    \"auth_config\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication configuration for the target endpoint.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"bearer_token\",\n            \"api_key_header\",\n            \"basic\",\n            \"none\"\n          ],\n          \"description\": \"Authentication method.\"\n        },\n        \"header_name\": {\n          \"type\": \"string\",\n          \"description\": \"Header name for API key authentication.\"\n        },\n        \"credential\": {\n          \"type\": \"string\",\n          \"description\": \"Authentication credential value\
  \ (API key or token).\",\n          \"writeOnly\": true\n        }\n      }\n    },\n    \"system_prompt\": {\n      \"type\": \"string\",\n      \"description\": \"System prompt to include in requests to the target. Used to scope red teaming attacks to the intended application context.\",\n      \"maxLength\": 8192\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"endpoint_url\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-target-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ScanTargetRequest
---
