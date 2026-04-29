---
description: A baseline definition.
layout: schema
name: Baseline
properties_list:
- description: The ARN of the baseline.
  name: arn
  type: string
- description: A description of the baseline.
  name: description
  type: string
- description: The name of the baseline.
  name: name
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/baseline-schema.json
slug: baseline
source_filename: baseline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/baseline-schema.json\",\n  \"title\": \"Baseline\",\n  \"description\": \"A baseline definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the baseline.\",\n      \"example\": \"arn:aws:controltower:us-east-1::baseline/LZACCOUNTBASELINE\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the baseline.\",\n      \"example\": \"AWS Control Tower Account baseline\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the baseline.\",\n      \"example\": \"AWSControlTowerBaseline\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/baseline-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: Baseline
---
