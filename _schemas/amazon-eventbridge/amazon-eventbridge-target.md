---
description: Target schema from Amazon EventBridge API
layout: schema
name: Target
properties_list:
- description: The ID of the target.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the target.
  name: Arn
  type: string
- description: The Amazon Resource Name (ARN) of the IAM role.
  name: RoleArn
  type: string
- description: Valid JSON text passed to the target.
  name: Input
  type: string
- description: JSONPath to extract from the event and send to the target.
  name: InputPath
  type: string
- description: Settings to transform input before sending to the target.
  name: InputTransformer
  type: object
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-target-schema.json
slug: amazon-eventbridge-target
source_filename: amazon-eventbridge-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-target-schema.json\",\n  \"title\": \"Target\",\n  \"description\": \"Target schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the target.\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the target.\"\n    },\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the IAM role.\"\n    },\n    \"Input\": {\n      \"type\": \"string\",\n      \"description\": \"Valid JSON text passed to the target.\"\n    },\n    \"InputPath\": {\n      \"type\": \"string\",\n      \"description\": \"JSONPath to extract from the event and send to the target.\"\n    },\n\
  \    \"InputTransformer\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"InputPathsMap\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"InputTemplate\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"Settings to transform input before sending to the target.\"\n    }\n  },\n  \"required\": [\n    \"Id\",\n    \"Arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-target-schema.json
tags:
- Amazon Web Services
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: Target
---
