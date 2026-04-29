---
description: A key-value pair associated with an Amazon Web Services resource. In EventBridge, rules and event buses support tagging.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-tag-schema.json
slug: amazon-eventbridge-pipes-tag
source_filename: amazon-eventbridge-pipes-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A key-value pair associated with an Amazon Web Services resource. In EventBridge, rules and event buses support tagging.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \"A string you can use to assign a value. The combination of tag keys and values can help you organize and categorize your resources.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \"The value for the specified tag key.\"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-tag-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: Tag
---
