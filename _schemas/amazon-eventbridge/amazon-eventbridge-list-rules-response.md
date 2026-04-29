---
description: ListRulesResponse schema from Amazon EventBridge API
layout: schema
name: ListRulesResponse
properties_list:
- description: ''
  name: Rules
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-list-rules-response-schema.json
slug: amazon-eventbridge-list-rules-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-rules-response-schema.json\",\n  \"title\": \"ListRulesResponse\",\n  \"description\": \"ListRulesResponse schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Rule\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-rules-response-schema.json
tags:
- Amazon Web Services
- AWS
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: ListRulesResponse
---
