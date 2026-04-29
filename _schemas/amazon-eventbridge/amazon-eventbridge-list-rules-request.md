---
description: ListRulesRequest schema from Amazon EventBridge API
layout: schema
name: ListRulesRequest
properties_list:
- description: ''
  name: NamePrefix
  type: string
- description: ''
  name: EventBusName
  type: string
- description: ''
  name: NextToken
  type: string
- description: ''
  name: Limit
  type: integer
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-list-rules-request-schema.json
slug: amazon-eventbridge-list-rules-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-rules-request-schema.json\",\n  \"title\": \"ListRulesRequest\",\n  \"description\": \"ListRulesRequest schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NamePrefix\": {\n      \"type\": \"string\"\n    },\n    \"EventBusName\": {\n      \"type\": \"string\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"Limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-rules-request-schema.json
tags:
- Amazon Web Services
- AWS
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: ListRulesRequest
---
