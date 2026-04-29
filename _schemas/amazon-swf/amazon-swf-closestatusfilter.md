---
description: Used to filter the closed workflow executions in visibility APIs by their close status.
layout: schema
name: CloseStatusFilter
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-closestatusfilter-schema.json
slug: amazon-swf-closestatusfilter
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"status\"\n  ],\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloseStatus\"\n        },\n        {\n          \"description\": \" The close status that must match the close status of an execution for it to meet the criteria of this filter.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Used to filter the closed workflow executions in visibility APIs by their close status.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CloseStatusFilter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-closestatusfilter-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: CloseStatusFilter
---
