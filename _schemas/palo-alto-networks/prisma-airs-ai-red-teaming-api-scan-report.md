---
description: ScanReport schema from Palo Alto Networks Prisma AIRS AI Red Teaming API
layout: schema
name: ScanReport
properties_list:
- description: Unique identifier of the scan.
  name: scan_id
  type: string
- description: ID of the assessed target.
  name: target_id
  type: string
- description: Display name of the assessed target.
  name: target_name
  type: string
- description: Overall vulnerability risk score from 0.0 (no risk) to 10.0 (critical).
  name: overall_risk_score
  type: number
- description: Total number of attack probes executed.
  name: total_attacks_executed
  type: integer
- description: Total number of vulnerabilities discovered.
  name: vulnerabilities_found
  type: integer
- description: Vulnerability summary per attack category.
  name: category_summaries
  type: array
- description: Individual vulnerability findings.
  name: findings
  type: array
- description: Timestamp when the report was generated.
  name: generated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-ai-red-teaming-api-scan-report-schema.json
slug: prisma-airs-ai-red-teaming-api-scan-report
source_filename: prisma-airs-ai-red-teaming-api-scan-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanReport\",\n  \"description\": \"ScanReport schema from Palo Alto Networks Prisma AIRS AI Red Teaming API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-report-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scan_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the scan.\"\n    },\n    \"target_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the assessed target.\"\n    },\n    \"target_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the assessed target.\"\n    },\n    \"overall_risk_score\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Overall vulnerability risk score from 0.0 (no risk) to 10.0 (critical).\",\n      \"minimum\": 0.0,\n    \
  \  \"maximum\": 10.0\n    },\n    \"total_attacks_executed\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of attack probes executed.\"\n    },\n    \"vulnerabilities_found\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of vulnerabilities discovered.\"\n    },\n    \"category_summaries\": {\n      \"type\": \"array\",\n      \"description\": \"Vulnerability summary per attack category.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"category_id\": {\n            \"type\": \"string\"\n          },\n          \"category_name\": {\n            \"type\": \"string\"\n          },\n          \"attacks_executed\": {\n            \"type\": \"integer\"\n          },\n          \"vulnerabilities_found\": {\n            \"type\": \"integer\"\n          },\n          \"risk_score\": {\n            \"type\": \"number\",\n            \"format\": \"float\"\n          }\n        }\n      }\n    },\n    \"\
  findings\": {\n      \"type\": \"array\",\n      \"description\": \"Individual vulnerability findings.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"finding_id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier of the finding.\"\n          },\n          \"category_id\": {\n            \"type\": \"string\",\n            \"description\": \"Attack category identifier.\"\n          },\n          \"category_name\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable attack category name.\"\n          },\n          \"severity\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"informational\",\n              \"low\",\n              \"medium\",\n              \"high\",\n              \"critical\"\n            ],\n            \"description\": \"Severity level of the vulnerability.\"\n          },\n          \"title\": {\n            \"type\": \"string\"\
  ,\n            \"description\": \"Brief title describing the vulnerability.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Detailed description of the vulnerability and its impact.\"\n          },\n          \"attack_prompt\": {\n            \"type\": \"string\",\n            \"description\": \"The adversarial prompt that revealed the vulnerability.\"\n          },\n          \"model_response\": {\n            \"type\": \"string\",\n            \"description\": \"The AI model's response to the attack prompt, demonstrating the vulnerability. May be truncated.\"\n          },\n          \"remediation\": {\n            \"type\": \"string\",\n            \"description\": \"Recommended steps to mitigate the vulnerability.\"\n          }\n        }\n      }\n    },\n    \"generated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the report was generated.\"\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-ai-red-teaming-api-scan-report-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ScanReport
---
