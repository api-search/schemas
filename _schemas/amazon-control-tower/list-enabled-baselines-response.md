---
description: ListEnabledBaselinesResponse schema from AWS Control Tower API
layout: schema
name: ListEnabledBaselinesResponse
properties_list:
- description: ''
  name: enabledBaselines
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/list-enabled-baselines-response-schema.json
slug: list-enabled-baselines-response
source_filename: list-enabled-baselines-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/list-enabled-baselines-response-schema.json\",\n  \"title\": \"ListEnabledBaselinesResponse\",\n  \"description\": \"ListEnabledBaselinesResponse schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabledBaselines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EnabledBaselineSummary\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/list-enabled-baselines-response-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: ListEnabledBaselinesResponse
---
