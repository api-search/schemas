---
description: BPACheck schema from Palo Alto Networks AIOps for NGFW BPA API
layout: schema
name: BPACheck
properties_list:
- description: Unique identifier of the check.
  name: check_id
  type: string
- description: Best practice category this check belongs to.
  name: category
  type: string
- description: Name of the best practice check.
  name: name
  type: string
- description: Description of what this check evaluates.
  name: description
  type: string
- description: Result status of this check.
  name: status
  type: string
- description: Severity if this check fails.
  name: severity
  type: string
- description: Current configuration value found on the device.
  name: current_value
  type: string
- description: Recommended configuration value per best practices.
  name: recommended_value
  type: string
- description: Step-by-step remediation guidance for failed checks.
  name: remediation
  type: string
- description: Reference URLs with additional guidance.
  name: references
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/aiops-ngfw-bpa-api-bpa-check-schema.json
slug: aiops-ngfw-bpa-api-bpa-check
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BPACheck\",\n  \"description\": \"BPACheck schema from Palo Alto Networks AIOps for NGFW BPA API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/aiops-ngfw-bpa-api-bpa-check-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"check_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the check.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Best practice category this check belongs to.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the best practice check.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what this check evaluates.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pass\",\n        \"fail\",\n \
  \       \"not_applicable\"\n      ],\n      \"description\": \"Result status of this check.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"informational\",\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ],\n      \"description\": \"Severity if this check fails.\"\n    },\n    \"current_value\": {\n      \"type\": \"string\",\n      \"description\": \"Current configuration value found on the device.\"\n    },\n    \"recommended_value\": {\n      \"type\": \"string\",\n      \"description\": \"Recommended configuration value per best practices.\"\n    },\n    \"remediation\": {\n      \"type\": \"string\",\n      \"description\": \"Step-by-step remediation guidance for failed checks.\"\n    },\n    \"references\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"Reference URLs with additional guidance.\"\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/aiops-ngfw-bpa-api-bpa-check-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BPACheck
---
