---
description: An enabled baseline for a target organizational unit.
layout: schema
name: EnabledBaseline
properties_list:
- description: The ARN of the enabled baseline.
  name: arn
  type: string
- description: The baseline ARN.
  name: baselineIdentifier
  type: string
- description: The version of the baseline.
  name: baselineVersion
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: statusSummary
  type: object
- description: The ARN of the target organizational unit.
  name: targetIdentifier
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enabled-baseline-schema.json
slug: enabled-baseline
source_filename: enabled-baseline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-baseline-schema.json\",\n  \"title\": \"EnabledBaseline\",\n  \"description\": \"An enabled baseline for a target organizational unit.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the enabled baseline.\",\n      \"example\": \"arn:aws:controltower:us-east-1:123456789012:enabledbaseline/a1b2c3d4EXAMPLE\"\n    },\n    \"baselineIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The baseline ARN.\"\n    },\n    \"baselineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the baseline.\",\n      \"example\": \"2.0\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EnabledBaselineParameter\"\
  \n      }\n    },\n    \"statusSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lastOperationIdentifier\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"targetIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the target organizational unit.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-baseline-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnabledBaseline
---
