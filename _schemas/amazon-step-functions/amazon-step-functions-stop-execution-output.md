---
description: StopExecutionOutput schema from Amazon Step Functions API
layout: schema
name: StopExecutionOutput
properties_list:
- description: ''
  name: stopDate
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-stop-execution-output-schema.json
slug: amazon-step-functions-stop-execution-output
source_filename: amazon-step-functions-stop-execution-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-stop-execution-output-schema.json\",\n  \"title\": \"StopExecutionOutput\",\n  \"description\": \"StopExecutionOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stopDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the execution is stopped.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stopDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-stop-execution-output-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: StopExecutionOutput
---
