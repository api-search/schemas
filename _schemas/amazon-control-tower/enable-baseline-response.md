---
description: EnableBaselineResponse schema from AWS Control Tower API
layout: schema
name: EnableBaselineResponse
properties_list:
- description: The ARN of the EnabledBaseline resource.
  name: arn
  type: string
- description: The identifier of the asynchronous operation.
  name: operationIdentifier
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enable-baseline-response-schema.json
slug: enable-baseline-response
source_filename: enable-baseline-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enable-baseline-response-schema.json\",\n  \"title\": \"EnableBaselineResponse\",\n  \"description\": \"EnableBaselineResponse schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the EnabledBaseline resource.\",\n      \"example\": \"arn:aws:controltower:us-east-1:123456789012:enabledbaseline/a1b2c3d4EXAMPLE\"\n    },\n    \"operationIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the asynchronous operation.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-EXAMPLE99999\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enable-baseline-response-schema.json
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnableBaselineResponse
---
