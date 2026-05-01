---
description: Contains the count of tasks in a task list.
layout: schema
name: PendingTaskCount
properties_list:
- description: ''
  name: count
  type: object
- description: ''
  name: truncated
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-pendingtaskcount-schema.json
slug: amazon-swf-pendingtaskcount
source_filename: amazon-swf-pendingtaskcount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"count\"\n  ],\n  \"properties\": {\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The number of tasks in the task list.\"\n        }\n      ]\n    },\n    \"truncated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Truncated\"\n        },\n        {\n          \"description\": \"If set to true, indicates that the actual count was more than the maximum supported by this API and the count returned is the truncated value.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains the count of tasks in a task list.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"PendingTaskCount\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-pendingtaskcount-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: PendingTaskCount
---
