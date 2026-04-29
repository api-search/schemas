---
description: Contains details about the start of a task during an execution.
layout: schema
name: TaskStartedEventDetails
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resource
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-task-started-event-details-schema.json
slug: amazon-step-functions-task-started-event-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-task-started-event-details-schema.json\",\n  \"title\": \"TaskStartedEventDetails\",\n  \"description\": \"Contains details about the start of a task during an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The service name of the resource in a task state.\"\n        }\n      ]\n    },\n    \"resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The action of the resource called by a task state.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-task-started-event-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: TaskStartedEventDetails
---
