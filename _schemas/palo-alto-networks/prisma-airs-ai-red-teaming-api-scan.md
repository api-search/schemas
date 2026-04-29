---
description: Scan schema from Palo Alto Networks Prisma AIRS AI Red Teaming API
layout: schema
name: Scan
properties_list:
- description: Unique identifier of the scan.
  name: scan_id
  type: string
- description: ID of the scan target being assessed.
  name: target_id
  type: string
- description: Display name of the scan target.
  name: target_name
  type: string
- description: Current status of the scan.
  name: status
  type: string
- description: Attack categories included in this scan.
  name: attack_categories
  type: array
- description: Scan completion progress from 0.0 to 1.0.
  name: progress
  type: number
- description: Total number of attack probes to be executed.
  name: total_attacks
  type: integer
- description: Number of attack probes completed so far.
  name: completed_attacks
  type: integer
- description: Number of vulnerabilities discovered so far.
  name: vulnerabilities_found
  type: integer
- description: Error description if the scan failed.
  name: error_message
  type: string
- description: Timestamp when the scan started.
  name: started_at
  type: string
- description: Timestamp when the scan completed.
  name: completed_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-ai-red-teaming-api-scan-schema.json
slug: prisma-airs-ai-red-teaming-api-scan
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Scan\",\n  \"description\": \"Scan schema from Palo Alto Networks Prisma AIRS AI Red Teaming API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scan_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the scan.\"\n    },\n    \"target_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the scan target being assessed.\"\n    },\n    \"target_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the scan target.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"running\",\n        \"completed\",\n        \"failed\",\n        \"cancelled\"\n      ],\n      \"description\": \"Current status of the\
  \ scan.\"\n    },\n    \"attack_categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Attack categories included in this scan.\"\n    },\n    \"progress\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Scan completion progress from 0.0 to 1.0.\",\n      \"minimum\": 0.0,\n      \"maximum\": 1.0\n    },\n    \"total_attacks\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of attack probes to be executed.\"\n    },\n    \"completed_attacks\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of attack probes completed so far.\"\n    },\n    \"vulnerabilities_found\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of vulnerabilities discovered so far.\"\n    },\n    \"error_message\": {\n      \"type\": \"string\",\n      \"description\": \"Error description if the scan failed.\"\n    },\n    \"started_at\": {\n    \
  \  \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the scan started.\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the scan completed.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Scan
---
