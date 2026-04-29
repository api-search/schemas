---
description: Contains details about the successful completion of a task state.
layout: schema
name: TaskSucceededEventDetails
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resource
  type: object
- description: ''
  name: output
  type: object
- description: ''
  name: outputDetails
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-task-succeeded-event-details-schema.json
slug: amazon-step-functions-task-succeeded-event-details
source_filename: amazon-step-functions-task-succeeded-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-task-succeeded-event-details-schema.json\",\n  \"title\": \"TaskSucceededEventDetails\",\n  \"description\": \"Contains details about the successful completion of a task state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The service name of the resource in a task state.\"\n        }\n      ]\n    },\n    \"resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The action of the resource called by a task state.\"\n        }\n      ]\n    },\n    \"output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\
  \n        },\n        {\n          \"description\": \"The full JSON response from a resource when a task has succeeded. This response becomes the output of the related task. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.\"\n        }\n      ]\n    },\n    \"outputDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoryEventExecutionDataDetails\"\n        },\n        {\n          \"description\": \"Contains details about the output of an execution history event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-task-succeeded-event-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: TaskSucceededEventDetails
---
