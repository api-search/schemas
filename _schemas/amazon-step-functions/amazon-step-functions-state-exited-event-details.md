---
description: Contains details about an exit from a state during an execution.
layout: schema
name: StateExitedEventDetails
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: output
  type: object
- description: ''
  name: outputDetails
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-state-exited-event-details-schema.json
slug: amazon-step-functions-state-exited-event-details
source_filename: amazon-step-functions-state-exited-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-state-exited-event-details-schema.json\",\n  \"title\": \"StateExitedEventDetails\",\n  \"description\": \"Contains details about an exit from a state during an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>The name of the state.</p> <p>A name must <i>not</i> contain:</p> <ul> <li> <p>white space</p> </li> <li> <p>brackets <code>&lt; &gt; { } [ ]</code> </p> </li> <li> <p>wildcard characters <code>? *</code> </p> </li> <li> <p>special characters <code>\\\" # % \\\\ ^ | ~ ` $ &amp; , ; : /</code> </p> </li> <li> <p>control characters (<code>U+0000-001F</code>, <code>U+007F-009F</code>)</p> </li> </ul> <p>To enable\
  \ logging with CloudWatch Logs, the name should only contain 0-9, A-Z, a-z, - and _.</p>\"\n        }\n      ]\n    },\n    \"output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\n        },\n        {\n          \"description\": \"The JSON output data of the state. Length constraints apply to the payload size, and are expressed as bytes in UTF-8 encoding.\"\n        }\n      ]\n    },\n    \"outputDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoryEventExecutionDataDetails\"\n        },\n        {\n          \"description\": \"Contains details about the output of an execution history event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-state-exited-event-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: StateExitedEventDetails
---
