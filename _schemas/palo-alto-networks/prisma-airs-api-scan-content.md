---
description: ScanContent schema from Palo Alto Networks Prisma AIRS API
layout: schema
name: ScanContent
properties_list:
- description: The user prompt or input text sent to the AI model. Evaluated for prompt injection, jailbreak attempts, and other input-side threats.
  name: prompt
  type: string
- description: The AI model response or output text. When provided, also evaluated for data leakage, toxic content, and other output-side threats. May be omitted to scan only the prompt.
  name: response
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-api-scan-content-schema.json
slug: prisma-airs-api-scan-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanContent\",\n  \"description\": \"ScanContent schema from Palo Alto Networks Prisma AIRS API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-scan-content-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"The user prompt or input text sent to the AI model. Evaluated for prompt injection, jailbreak attempts, and other input-side threats.\",\n      \"maxLength\": 32000\n    },\n    \"response\": {\n      \"type\": \"string\",\n      \"description\": \"The AI model response or output text. When provided, also evaluated for data leakage, toxic content, and other output-side threats. May be omitted to scan only the prompt.\",\n      \"maxLength\": 64000\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-scan-content-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ScanContent
---
