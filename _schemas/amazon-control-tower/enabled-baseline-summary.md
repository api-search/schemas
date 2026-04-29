---
description: Summary of an enabled baseline.
layout: schema
name: EnabledBaselineSummary
properties_list:
- description: ''
  name: arn
  type: string
- description: ''
  name: baselineIdentifier
  type: string
- description: ''
  name: statusSummary
  type: object
- description: ''
  name: targetIdentifier
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enabled-baseline-summary-schema.json
slug: enabled-baseline-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-baseline-summary-schema.json\",\n  \"title\": \"EnabledBaselineSummary\",\n  \"description\": \"Summary of an enabled baseline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\"\n    },\n    \"baselineIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"statusSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"targetIdentifier\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-baseline-summary-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnabledBaselineSummary
---
