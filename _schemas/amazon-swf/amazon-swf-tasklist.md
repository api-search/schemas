---
description: Represents a task list.
layout: schema
name: TaskList
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-tasklist-schema.json
slug: amazon-swf-tasklist
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the task list.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents a task list.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TaskList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-tasklist-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: TaskList
---
