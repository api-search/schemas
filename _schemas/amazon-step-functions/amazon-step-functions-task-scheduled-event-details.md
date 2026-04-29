---
description: Contains details about a task scheduled during an execution.
layout: schema
name: TaskScheduledEventDetails
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resource
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: parameters
  type: object
- description: ''
  name: timeoutInSeconds
  type: object
- description: ''
  name: heartbeatInSeconds
  type: object
- description: ''
  name: taskCredentials
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-task-scheduled-event-details-schema.json
slug: amazon-step-functions-task-scheduled-event-details
source_filename: amazon-step-functions-task-scheduled-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-task-scheduled-event-details-schema.json\",\n  \"title\": \"TaskScheduledEventDetails\",\n  \"description\": \"Contains details about a task scheduled during an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The service name of the resource in a task state.\"\n        }\n      ]\n    },\n    \"resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The action of the resource called by a task state.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\
  \n        },\n        {\n          \"description\": \"The region of the scheduled task\"\n        }\n      ]\n    },\n    \"parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectorParameters\"\n        },\n        {\n          \"description\": \"The JSON data passed to the resource referenced in a task state. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.\"\n        }\n      ]\n    },\n    \"timeoutInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeoutInSeconds\"\n        },\n        {\n          \"description\": \"The maximum allowed duration of the task.\"\n        }\n      ]\n    },\n    \"heartbeatInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeoutInSeconds\"\n        },\n        {\n          \"description\": \"The maximum allowed duration between two heartbeats for the task.\"\n        }\n      ]\n    },\n\
  \    \"taskCredentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskCredentials\"\n        },\n        {\n          \"description\": \"The credentials that Step Functions uses for the task.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resource\",\n    \"region\",\n    \"parameters\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-task-scheduled-event-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: TaskScheduledEventDetails
---
