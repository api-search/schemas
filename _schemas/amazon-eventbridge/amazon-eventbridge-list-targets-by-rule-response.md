---
description: ListTargetsByRuleResponse schema from Amazon EventBridge API
layout: schema
name: ListTargetsByRuleResponse
properties_list:
- description: ''
  name: Targets
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-list-targets-by-rule-response-schema.json
slug: amazon-eventbridge-list-targets-by-rule-response
source_filename: amazon-eventbridge-list-targets-by-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-targets-by-rule-response-schema.json\",\n  \"title\": \"ListTargetsByRuleResponse\",\n  \"description\": \"ListTargetsByRuleResponse schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Targets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Target\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-targets-by-rule-response-schema.json
tags:
- Amazon Web Services
- AWS
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: ListTargetsByRuleResponse
---
