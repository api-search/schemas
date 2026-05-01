---
description: A <code>DeadLetterConfig</code> object that contains information about a dead-letter queue configuration.
layout: schema
name: DeadLetterConfig
properties_list:
- description: ''
  name: Arn
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-dead-letter-config-schema.json
slug: amazon-eventbridge-pipes-dead-letter-config
source_filename: amazon-eventbridge-pipes-dead-letter-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-dead-letter-config-schema.json\",\n  \"title\": \"DeadLetterConfig\",\n  \"description\": \"A <code>DeadLetterConfig</code> object that contains information about a dead-letter queue configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the Amazon SQS queue specified as the target for the dead-letter queue.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-dead-letter-config-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: DeadLetterConfig
---
