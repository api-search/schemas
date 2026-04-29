---
description: BPAReport schema from Palo Alto Networks AIOps for NGFW BPA API
layout: schema
name: BPAReport
properties_list:
- description: Unique identifier of the report.
  name: report_id
  type: string
- description: ID of the BPA request that generated this report.
  name: request_id
  type: string
- description: Device serial number assessed.
  name: serial_number
  type: string
- description: PAN-OS version assessed.
  name: pan_os_version
  type: string
- description: Overall best practice compliance score from 0.0 to 100.0.
  name: overall_score
  type: number
- description: Compliance scores broken down by best practice category.
  name: category_scores
  type: array
- description: Total number of checks evaluated.
  name: total_checks
  type: integer
- description: Number of checks that passed.
  name: passed_checks
  type: integer
- description: Number of checks that failed.
  name: failed_checks
  type: integer
- description: Timestamp when the report was generated.
  name: generated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/aiops-ngfw-bpa-api-bpa-report-schema.json
slug: aiops-ngfw-bpa-api-bpa-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BPAReport\",\n  \"description\": \"BPAReport schema from Palo Alto Networks AIOps for NGFW BPA API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/aiops-ngfw-bpa-api-bpa-report-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"report_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the report.\"\n    },\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the BPA request that generated this report.\"\n    },\n    \"serial_number\": {\n      \"type\": \"string\",\n      \"description\": \"Device serial number assessed.\"\n    },\n    \"pan_os_version\": {\n      \"type\": \"string\",\n      \"description\": \"PAN-OS version assessed.\"\n    },\n    \"overall_score\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\"\
  : \"Overall best practice compliance score from 0.0 to 100.0.\",\n      \"minimum\": 0.0,\n      \"maximum\": 100.0\n    },\n    \"category_scores\": {\n      \"type\": \"array\",\n      \"description\": \"Compliance scores broken down by best practice category.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"category\": {\n            \"type\": \"string\",\n            \"description\": \"Best practice category name.\"\n          },\n          \"score\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"description\": \"Category compliance score (0.0 to 100.0).\"\n          },\n          \"passed\": {\n            \"type\": \"integer\",\n            \"description\": \"Number of checks that passed in this category.\"\n          },\n          \"failed\": {\n            \"type\": \"integer\",\n            \"description\": \"Number of checks that failed in this category.\"\n          },\n          \"not_applicable\"\
  : {\n            \"type\": \"integer\",\n            \"description\": \"Number of checks not applicable to this device.\"\n          }\n        }\n      }\n    },\n    \"total_checks\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of checks evaluated.\"\n    },\n    \"passed_checks\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of checks that passed.\"\n    },\n    \"failed_checks\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of checks that failed.\"\n    },\n    \"generated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the report was generated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/aiops-ngfw-bpa-api-bpa-report-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BPAReport
---
