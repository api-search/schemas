---
description: A safety mechanism that can stop or prevent FIS experiments
layout: schema
name: SafetyLever
properties_list:
- description: Safety lever ID
  name: id
  type: string
- description: Safety lever ARN
  name: arn
  type: string
- description: ''
  name: state
  type: object
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-safety-lever-schema.json
slug: amazon-fis-safety-lever
source_filename: amazon-fis-safety-lever-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-safety-lever-schema.json\",\n  \"title\": \"SafetyLever\",\n  \"description\": \"A safety mechanism that can stop or prevent FIS experiments\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Safety lever ID\",\n      \"example\": \"SL123\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"Safety lever ARN\",\n      \"example\": \"arn:aws:fis:us-east-1:123456789012:safety-lever/SL123\"\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/SafetyLeverState\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-safety-lever-schema.json
tags:
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: SafetyLever
---
