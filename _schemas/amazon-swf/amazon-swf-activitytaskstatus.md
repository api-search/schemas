---
description: Status information about an activity task.
layout: schema
name: ActivityTaskStatus
properties_list:
- description: ''
  name: cancelRequested
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytaskstatus-schema.json
slug: amazon-swf-activitytaskstatus
source_filename: amazon-swf-activitytaskstatus-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"cancelRequested\"\n  ],\n  \"properties\": {\n    \"cancelRequested\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Canceled\"\n        },\n        {\n          \"description\": \"Set to <code>true</code> if cancellation of the task is requested.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Status information about an activity task.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ActivityTaskStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytaskstatus-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ActivityTaskStatus
---
