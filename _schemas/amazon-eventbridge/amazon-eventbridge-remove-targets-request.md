---
description: RemoveTargetsRequest schema from Amazon EventBridge API
layout: schema
name: RemoveTargetsRequest
properties_list:
- description: ''
  name: Rule
  type: string
- description: ''
  name: EventBusName
  type: string
- description: ''
  name: Ids
  type: array
- description: ''
  name: Force
  type: boolean
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-remove-targets-request-schema.json
slug: amazon-eventbridge-remove-targets-request
source_filename: amazon-eventbridge-remove-targets-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-remove-targets-request-schema.json\",\n  \"title\": \"RemoveTargetsRequest\",\n  \"description\": \"RemoveTargetsRequest schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rule\": {\n      \"type\": \"string\"\n    },\n    \"EventBusName\": {\n      \"type\": \"string\"\n    },\n    \"Ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"Force\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"Rule\",\n    \"Ids\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-remove-targets-request-schema.json
tags:
- Amazon Web Services
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: RemoveTargetsRequest
---
