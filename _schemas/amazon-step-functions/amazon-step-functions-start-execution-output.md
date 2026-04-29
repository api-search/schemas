---
description: StartExecutionOutput schema from Amazon Step Functions API
layout: schema
name: StartExecutionOutput
properties_list:
- description: ''
  name: executionArn
  type: object
- description: ''
  name: startDate
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-start-execution-output-schema.json
slug: amazon-step-functions-start-execution-output
source_filename: amazon-step-functions-start-execution-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-start-execution-output-schema.json\",\n  \"title\": \"StartExecutionOutput\",\n  \"description\": \"StartExecutionOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the execution.\"\n        }\n      ]\n    },\n    \"startDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the execution is started.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"executionArn\",\n    \"startDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-start-execution-output-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: StartExecutionOutput
---
