---
description: GetActivityTaskOutput schema from Amazon Step Functions API
layout: schema
name: GetActivityTaskOutput
properties_list:
- description: ''
  name: taskToken
  type: object
- description: ''
  name: input
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-get-activity-task-output-schema.json
slug: amazon-step-functions-get-activity-task-output
source_filename: amazon-step-functions-get-activity-task-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-get-activity-task-output-schema.json\",\n  \"title\": \"GetActivityTaskOutput\",\n  \"description\": \"GetActivityTaskOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskToken\"\n        },\n        {\n          \"description\": \"A token that identifies the scheduled task. This token must be copied and included in subsequent calls to <a>SendTaskHeartbeat</a>, <a>SendTaskSuccess</a> or <a>SendTaskFailure</a> in order to report the progress or completion of the task.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveDataJobInput\"\n        },\n        {\n\
  \          \"description\": \"The string that contains the JSON input data for the task. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-get-activity-task-output-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: GetActivityTaskOutput
---
