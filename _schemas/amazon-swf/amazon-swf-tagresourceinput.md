---
description: ''
layout: schema
name: TagResourceInput
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-tagresourceinput-schema.json
slug: amazon-swf-tagresourceinput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"resourceArn\",\n    \"tags\"\n  ],\n  \"title\": \"TagResourceInput\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the Amazon SWF domain.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTagList\"\n        },\n        {\n          \"description\": \"<p>The list of tags to add to a domain. </p> <p>Tags may only contain unicode letters, digits, whitespace, or these symbols: <code>_ . : / = + - @</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-tagresourceinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: TagResourceInput
---
