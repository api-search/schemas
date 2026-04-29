---
description: The action required to resolve a broker issue when the broker is in a CRITICAL_ACTION_REQUIRED state.
layout: schema
name: ActionRequired
properties_list:
- description: ''
  name: ActionRequiredCode
  type: object
- description: ''
  name: ActionRequiredInfo
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-action-required-schema.json
slug: mq-api-action-required
source_filename: mq-api-action-required-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-action-required-schema.json\",\n  \"title\": \"ActionRequired\",\n  \"description\": \"The action required to resolve a broker issue when the broker is in a CRITICAL_ACTION_REQUIRED state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionRequiredCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"actionRequiredCode\"\n          },\n          \"description\": \"The code you can use to resolve your broker issue when the broker is in a CRITICAL_ACTION_REQUIRED state. You can find instructions by choosing the link for your code from the list of action required codes in <a href=\\\"https://docs.aws.amazon.com//latest/developer-guide/troubleshooting-action-required-codes.html\\\">Amazon\
  \ MQ action required codes</a>. Each code references a topic with detailed information, instructions, and recommendations for how to resolve the issue and prevent future occurrences.\"\n        }\n      ]\n    },\n    \"ActionRequiredInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"actionRequiredInfo\"\n          },\n          \"description\": \"Information about the action required to resolve your broker issue when the broker is in a CRITICAL_ACTION_REQUIRED state.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-action-required-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ActionRequired
---
