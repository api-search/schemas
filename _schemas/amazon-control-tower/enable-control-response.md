---
description: EnableControlResponse schema from AWS Control Tower API
layout: schema
name: EnableControlResponse
properties_list:
- description: The ARN of the EnabledControl resource.
  name: arn
  type: string
- description: The identifier of the asynchronous operation.
  name: operationIdentifier
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enable-control-response-schema.json
slug: enable-control-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enable-control-response-schema.json\",\n  \"title\": \"EnableControlResponse\",\n  \"description\": \"EnableControlResponse schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the EnabledControl resource.\",\n      \"example\": \"arn:aws:controltower:us-east-1:123456789012:enabledcontrol/a1b2c3d4EXAMPLE\"\n    },\n    \"operationIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the asynchronous operation.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-EXAMPLE55555\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enable-control-response-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnableControlResponse
---
