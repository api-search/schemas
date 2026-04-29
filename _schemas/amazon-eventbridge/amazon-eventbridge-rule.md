---
description: Rule schema from Amazon EventBridge API
layout: schema
name: Rule
properties_list:
- description: The name of the rule.
  name: Name
  type: string
- description: The Amazon Resource Name (ARN) of the rule.
  name: Arn
  type: string
- description: The event pattern of the rule.
  name: EventPattern
  type: string
- description: The state of the rule.
  name: State
  type: string
- description: The description of the rule.
  name: Description
  type: string
- description: The scheduling expression (e.g., cron or rate expression).
  name: ScheduleExpression
  type: string
- description: The Amazon Resource Name (ARN) of the IAM role.
  name: RoleArn
  type: string
- description: The name or ARN of the event bus associated with the rule.
  name: EventBusName
  type: string
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-rule-schema.json
slug: amazon-eventbridge-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-rule-schema.json\",\n  \"title\": \"Rule\",\n  \"description\": \"Rule schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the rule.\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the rule.\"\n    },\n    \"EventPattern\": {\n      \"type\": \"string\",\n      \"description\": \"The event pattern of the rule.\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ],\n      \"description\": \"The state of the rule.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the rule.\"\
  \n    },\n    \"ScheduleExpression\": {\n      \"type\": \"string\",\n      \"description\": \"The scheduling expression (e.g., cron or rate expression).\"\n    },\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the IAM role.\"\n    },\n    \"EventBusName\": {\n      \"type\": \"string\",\n      \"description\": \"The name or ARN of the event bus associated with the rule.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-rule-schema.json
tags:
- Amazon Web Services
- AWS
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: Rule
---
