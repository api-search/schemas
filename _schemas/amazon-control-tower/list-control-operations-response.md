---
description: ListControlOperationsResponse schema from AWS Control Tower API
layout: schema
name: ListControlOperationsResponse
properties_list:
- description: ''
  name: controlOperations
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/list-control-operations-response-schema.json
slug: list-control-operations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/list-control-operations-response-schema.json\",\n  \"title\": \"ListControlOperationsResponse\",\n  \"description\": \"ListControlOperationsResponse schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"controlOperations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ControlOperationSummary\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/list-control-operations-response-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: ListControlOperationsResponse
---
