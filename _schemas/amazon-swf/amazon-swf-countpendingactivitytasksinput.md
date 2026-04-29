---
description: ''
layout: schema
name: CountPendingActivityTasksInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: taskList
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-countpendingactivitytasksinput-schema.json
slug: amazon-swf-countpendingactivitytasksinput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"taskList\"\n  ],\n  \"title\": \"CountPendingActivityTasksInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain that contains the task list.\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"The name of the task list.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-countpendingactivitytasksinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: CountPendingActivityTasksInput
---
