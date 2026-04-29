---
description: Summary information about an enabled control.
layout: schema
name: EnabledControlSummary
properties_list:
- description: The ARN of the enabled control.
  name: arn
  type: string
- description: The control identifier.
  name: controlIdentifier
  type: string
- description: ''
  name: statusSummary
  type: object
- description: ''
  name: targetIdentifier
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enabled-control-summary-schema.json
slug: enabled-control-summary
source_filename: enabled-control-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-control-summary-schema.json\",\n  \"title\": \"EnabledControlSummary\",\n  \"description\": \"Summary information about an enabled control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the enabled control.\"\n    },\n    \"controlIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The control identifier.\"\n    },\n    \"statusSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"targetIdentifier\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-control-summary-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnabledControlSummary
---
