---
description: PutRuleRequest schema from Amazon EventBridge API
layout: schema
name: PutRuleRequest
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: EventPattern
  type: string
- description: ''
  name: ScheduleExpression
  type: string
- description: ''
  name: State
  type: string
- description: ''
  name: RoleArn
  type: string
- description: ''
  name: EventBusName
  type: string
- description: ''
  name: Tags
  type: array
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-put-rule-request-schema.json
slug: amazon-eventbridge-put-rule-request
source_filename: amazon-eventbridge-put-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-put-rule-request-schema.json\",\n  \"title\": \"PutRuleRequest\",\n  \"description\": \"PutRuleRequest schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"EventPattern\": {\n      \"type\": \"string\"\n    },\n    \"ScheduleExpression\": {\n      \"type\": \"string\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ]\n    },\n    \"RoleArn\": {\n      \"type\": \"string\"\n    },\n    \"EventBusName\": {\n      \"type\": \"string\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"Key\": {\n            \"type\": \"string\"\n          },\n          \"Value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-put-rule-request-schema.json
tags:
- Amazon Web Services
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: PutRuleRequest
---
