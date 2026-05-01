---
description: DeleteRuleRequest schema from Amazon EventBridge API
layout: schema
name: DeleteRuleRequest
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: EventBusName
  type: string
- description: ''
  name: Force
  type: boolean
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-delete-rule-request-schema.json
slug: amazon-eventbridge-delete-rule-request
source_filename: amazon-eventbridge-delete-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-delete-rule-request-schema.json\",\n  \"title\": \"DeleteRuleRequest\",\n  \"description\": \"DeleteRuleRequest schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"EventBusName\": {\n      \"type\": \"string\"\n    },\n    \"Force\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-delete-rule-request-schema.json
tags:
- Amazon Web Services
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: DeleteRuleRequest
---
