---
description: State of a safety lever
layout: schema
name: SafetyLeverState
properties_list:
- description: Safety lever status
  name: status
  type: string
- description: Status reason
  name: reason
  type: string
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-safety-lever-state-schema.json
slug: amazon-fis-safety-lever-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-safety-lever-state-schema.json\",\n  \"title\": \"SafetyLeverState\",\n  \"description\": \"State of a safety lever\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Safety lever status\",\n      \"example\": \"engaged\",\n      \"enum\": [\n        \"engaged\",\n        \"disengaged\",\n        \"engaging\",\n        \"disengaging\"\n      ]\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Status reason\",\n      \"example\": \"No active experiments\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-safety-lever-state-schema.json
tags:
- AWS
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: SafetyLeverState
---
