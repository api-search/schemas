---
description: ''
layout: schema
name: ListTagsForResourceInput
properties_list:
- description: ''
  name: resourceArn
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-listtagsforresourceinput-schema.json
slug: amazon-swf-listtagsforresourceinput
source_filename: amazon-swf-listtagsforresourceinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"resourceArn\"\n  ],\n  \"title\": \"ListTagsForResourceInput\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the Amazon SWF domain.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-listtagsforresourceinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ListTagsForResourceInput
---
