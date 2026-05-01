---
description: GetActivityTaskInput schema from Amazon Step Functions API
layout: schema
name: GetActivityTaskInput
properties_list:
- description: ''
  name: activityArn
  type: object
- description: ''
  name: workerName
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-get-activity-task-input-schema.json
slug: amazon-step-functions-get-activity-task-input
source_filename: amazon-step-functions-get-activity-task-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-get-activity-task-input-schema.json\",\n  \"title\": \"GetActivityTaskInput\",\n  \"description\": \"GetActivityTaskInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the activity to retrieve tasks from (assigned when you create the task using <a>CreateActivity</a>.)\"\n        }\n      ]\n    },\n    \"workerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"You can provide an arbitrary name in order to identify the worker that the task is assigned to.\
  \ This name is used when it is logged in the execution history.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"activityArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-get-activity-task-input-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: GetActivityTaskInput
---
