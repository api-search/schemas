---
description: BPARequestStatus schema from Palo Alto Networks AIOps for NGFW BPA API
layout: schema
name: BPARequestStatus
properties_list:
- description: Unique identifier of the BPA request.
  name: request_id
  type: string
- description: Device serial number for which the assessment was submitted.
  name: serial_number
  type: string
- description: Current processing status of the request.
  name: status
  type: string
- description: Report identifier available when status is completed. Use with GET /reports/{report_id} to retrieve the full report.
  name: report_id
  type: string
- description: Error description when status is failed.
  name: error_message
  type: string
- description: Timestamp when the request was submitted.
  name: submitted_at
  type: string
- description: Timestamp when processing completed.
  name: completed_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/aiops-ngfw-bpa-api-bpa-request-status-schema.json
slug: aiops-ngfw-bpa-api-bpa-request-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BPARequestStatus\",\n  \"description\": \"BPARequestStatus schema from Palo Alto Networks AIOps for NGFW BPA API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/aiops-ngfw-bpa-api-bpa-request-status-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the BPA request.\"\n    },\n    \"serial_number\": {\n      \"type\": \"string\",\n      \"description\": \"Device serial number for which the assessment was submitted.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"description\": \"Current processing status of the request.\"\n    },\n    \"report_id\": {\n      \"type\": \"string\",\n  \
  \    \"description\": \"Report identifier available when status is completed. Use with GET /reports/{report_id} to retrieve the full report.\"\n    },\n    \"error_message\": {\n      \"type\": \"string\",\n      \"description\": \"Error description when status is failed.\"\n    },\n    \"submitted_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the request was submitted.\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when processing completed.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/aiops-ngfw-bpa-api-bpa-request-status-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BPARequestStatus
---
