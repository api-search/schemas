---
description: Contains details about a state entered during an execution.
layout: schema
name: StateEnteredEventDetails
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: inputDetails
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-state-entered-event-details-schema.json
slug: amazon-step-functions-state-entered-event-details
source_filename: amazon-step-functions-state-entered-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-state-entered-event-details-schema.json\",\n  \"title\": \"StateEnteredEventDetails\",\n  \"description\": \"Contains details about a state entered during an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the state.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"The string that contains the JSON input data for the state. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.\"\n        }\n      ]\n    },\n    \"inputDetails\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoryEventExecutionDataDetails\"\n        },\n        {\n          \"description\": \"Contains details about the input for an execution history event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-state-entered-event-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: StateEnteredEventDetails
---
