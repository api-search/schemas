---
description: ''
layout: schema
name: StartSyncExecutionInput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: traceHeader
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-startsyncexecutioninput-schema.json
slug: step-functions-startsyncexecutioninput
source_filename: step-functions-startsyncexecutioninput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StartSyncExecutionInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {},\n    \"name\": {},\n    \"input\": {},\n    \"traceHeader\": {}\n  },\n  \"required\": [\n    \"stateMachineArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-startsyncexecutioninput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: StartSyncExecutionInput
---
