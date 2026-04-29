---
description: ScanRequest schema from Palo Alto Networks Prisma AIRS AI Red Teaming API
layout: schema
name: ScanRequest
properties_list:
- description: ID of the scan target to assess.
  name: target_id
  type: string
- description: Attack category identifiers to include in the scan. Use GET /v1/attack-categories to retrieve available category IDs.
  name: attack_categories
  type: array
- description: Optional custom adversarial prompts to include alongside the built-in attack library. Useful for testing application-specific threat scenarios.
  name: custom_prompts
  type: array
- description: Maximum number of attack probes per category. Limits scan duration for large attack libraries. If omitted, all available attacks for each category are executed.
  name: max_attacks_per_category
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-ai-red-teaming-api-scan-request-schema.json
slug: prisma-airs-ai-red-teaming-api-scan-request
source_filename: prisma-airs-ai-red-teaming-api-scan-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanRequest\",\n  \"description\": \"ScanRequest schema from Palo Alto Networks Prisma AIRS AI Red Teaming API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"target_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the scan target to assess.\"\n    },\n    \"attack_categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"description\": \"Attack category identifiers to include in the scan. Use GET /v1/attack-categories to retrieve available category IDs.\"\n    },\n    \"custom_prompts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Optional custom adversarial\
  \ prompts to include alongside the built-in attack library. Useful for testing application-specific threat scenarios.\",\n      \"maxItems\": 100\n    },\n    \"max_attacks_per_category\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of attack probes per category. Limits scan duration for large attack libraries. If omitted, all available attacks for each category are executed.\",\n      \"minimum\": 1,\n      \"maximum\": 1000\n    }\n  },\n  \"required\": [\n    \"target_id\",\n    \"attack_categories\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-request-schema.json
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
