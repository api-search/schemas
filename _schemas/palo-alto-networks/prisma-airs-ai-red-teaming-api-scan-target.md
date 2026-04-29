---
description: ScanTarget schema from Palo Alto Networks Prisma AIRS AI Red Teaming API
layout: schema
name: ScanTarget
properties_list:
- description: Unique identifier of the scan target.
  name: target_id
  type: string
- description: Display name of the scan target.
  name: name
  type: string
- description: Description of the target AI application.
  name: description
  type: string
- description: AI interface type of the target endpoint.
  name: type
  type: string
- description: URL of the AI application endpoint.
  name: endpoint_url
  type: string
- description: AI model name or identifier used by the endpoint.
  name: model
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-ai-red-teaming-api-scan-target-schema.json
slug: prisma-airs-ai-red-teaming-api-scan-target
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanTarget\",\n  \"description\": \"ScanTarget schema from Palo Alto Networks Prisma AIRS AI Red Teaming API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-target-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"target_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the scan target.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the scan target.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the target AI application.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"openai_chat\",\n        \"anthropic_messages\",\n        \"custom_http\",\n        \"huggingface\"\n      ],\n      \"description\"\
  : \"AI interface type of the target endpoint.\"\n    },\n    \"endpoint_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the AI application endpoint.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"AI model name or identifier used by the endpoint.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-target-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ScanTarget
---
