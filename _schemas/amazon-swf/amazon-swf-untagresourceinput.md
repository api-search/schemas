---
description: ''
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: tagKeys
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-untagresourceinput-schema.json
slug: amazon-swf-untagresourceinput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"resourceArn\",\n    \"tagKeys\"\n  ],\n  \"title\": \"UntagResourceInput\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the Amazon SWF domain.\"\n        }\n      ]\n    },\n    \"tagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTagKeyList\"\n        },\n        {\n          \"description\": \"The list of tags to remove from the Amazon SWF domain.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-untagresourceinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: UntagResourceInput
---
