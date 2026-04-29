---
description: ScanResponse schema from Palo Alto Networks Prisma AIRS API
layout: schema
name: ScanResponse
properties_list:
- description: Unique identifier of the scan.
  name: scan_id
  type: string
- description: Current or final status of the scan.
  name: status
  type: string
- description: Identifier for the detailed scan report.
  name: report_id
  type: string
- description: Highest severity threat category detected.
  name: scan_category
  type: string
- description: Per-content scan results corresponding to each submitted content item.
  name: results
  type: array
- description: Transaction ID echoed from the request if provided.
  name: tr_id
  type: string
- description: Timestamp when the scan was submitted.
  name: created_at
  type: string
- description: Timestamp when the scan completed.
  name: completed_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-api-scan-response-schema.json
slug: prisma-airs-api-scan-response
source_filename: prisma-airs-api-scan-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanResponse\",\n  \"description\": \"ScanResponse schema from Palo Alto Networks Prisma AIRS API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-scan-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scan_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the scan.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"completed\",\n        \"error\"\n      ],\n      \"description\": \"Current or final status of the scan.\"\n    },\n    \"report_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the detailed scan report.\"\n    },\n    \"scan_category\": {\n      \"type\": \"string\",\n      \"description\": \"Highest severity threat category detected.\"\
  \n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Per-content scan results corresponding to each submitted content item.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"prompt_detected\": {\n            \"type\": \"object\",\n            \"description\": \"Threats detected in the prompt field.\",\n            \"properties\": {\n              \"url_cats\": {\n                \"type\": \"boolean\",\n                \"description\": \"Malicious URL categories detected in prompt.\"\n              },\n              \"dlp\": {\n                \"type\": \"boolean\",\n                \"description\": \"Data loss prevention triggers in prompt.\"\n              },\n              \"injection\": {\n                \"type\": \"boolean\",\n                \"description\": \"Prompt injection detected.\"\n              }\n            }\n          },\n          \"response_detected\": {\n            \"type\": \"object\",\n \
  \           \"description\": \"Threats detected in the response field.\",\n            \"properties\": {\n              \"url_cats\": {\n                \"type\": \"boolean\",\n                \"description\": \"Malicious URL categories detected in response.\"\n              },\n              \"dlp\": {\n                \"type\": \"boolean\",\n                \"description\": \"Data loss prevention triggers in response.\"\n              },\n              \"toxic_content\": {\n                \"type\": \"boolean\",\n                \"description\": \"Toxic or harmful content detected in response.\"\n              }\n            }\n          },\n          \"verdict\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"benign\",\n              \"malicious\"\n            ],\n            \"description\": \"Overall verdict for this content pair.\"\n          },\n          \"action\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"allow\"\
  ,\n              \"block\"\n            ],\n            \"description\": \"Action taken based on the security profile configuration.\"\n          }\n        }\n      }\n    },\n    \"tr_id\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction ID echoed from the request if provided.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the scan was submitted.\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the scan completed.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-scan-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ScanResponse
---
