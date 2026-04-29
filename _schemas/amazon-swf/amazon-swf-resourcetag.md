---
description: '<p>Tags are key-value pairs that can be associated with Amazon SWF state machines and activities.</p> <p>Tags may only contain unicode letters, digits, whitespace, or these symbols: <code>_ . : / = + - @</code>.</p>'
layout: schema
name: ResourceTag
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-resourcetag-schema.json
slug: amazon-swf-resourcetag
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"key\"\n  ],\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTagKey\"\n        },\n        {\n          \"description\": \"The key of a tag.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTagValue\"\n        },\n        {\n          \"description\": \"The value of a tag.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>Tags are key-value pairs that can be associated with Amazon SWF state machines and activities.</p> <p>Tags may only contain unicode letters, digits, whitespace, or these symbols: <code>_ . : / = + - @</code>.</p>\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ResourceTag\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-resourcetag-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ResourceTag
---
