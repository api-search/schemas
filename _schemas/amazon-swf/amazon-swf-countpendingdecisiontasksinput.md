---
description: ''
layout: schema
name: CountPendingDecisionTasksInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: taskList
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-countpendingdecisiontasksinput-schema.json
slug: amazon-swf-countpendingdecisiontasksinput
source_filename: amazon-swf-countpendingdecisiontasksinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"taskList\"\n  ],\n  \"title\": \"CountPendingDecisionTasksInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain that contains the task list.\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"The name of the task list.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-countpendingdecisiontasksinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: CountPendingDecisionTasksInput
---
