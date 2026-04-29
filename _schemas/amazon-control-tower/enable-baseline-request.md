---
description: EnableBaselineRequest schema from AWS Control Tower API
layout: schema
name: EnableBaselineRequest
properties_list:
- description: The ARN of the baseline.
  name: baselineIdentifier
  type: string
- description: The specific version to be enabled.
  name: baselineVersion
  type: string
- description: A list of key-value objects that specify enablement parameters.
  name: parameters
  type: array
- description: Tags to apply to the EnabledBaseline resource.
  name: tags
  type: object
- description: The ARN of the target organizational unit.
  name: targetIdentifier
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enable-baseline-request-schema.json
slug: enable-baseline-request
source_filename: enable-baseline-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enable-baseline-request-schema.json\",\n  \"title\": \"EnableBaselineRequest\",\n  \"description\": \"EnableBaselineRequest schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baselineIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the baseline.\",\n      \"example\": \"arn:aws:controltower:us-east-1::baseline/LZACCOUNTBASELINE\"\n    },\n    \"baselineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The specific version to be enabled.\",\n      \"example\": \"2.0\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of key-value objects that specify enablement parameters.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EnabledBaselineParameter\"\n   \
  \   }\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags to apply to the EnabledBaseline resource.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"targetIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the target organizational unit.\",\n      \"example\": \"arn:aws:organizations::123456789012:ou/o-exampleorgid11/ou-exampleouid111\"\n    }\n  },\n  \"required\": [\n    \"baselineIdentifier\",\n    \"baselineVersion\",\n    \"targetIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enable-baseline-request-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnableBaselineRequest
---
