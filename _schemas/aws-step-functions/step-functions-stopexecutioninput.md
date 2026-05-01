---
description: ''
layout: schema
name: StopExecutionInput
properties_list:
- description: ''
  name: executionArn
  type: object
- description: ''
  name: error
  type: object
- description: ''
  name: cause
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-stopexecutioninput-schema.json
slug: step-functions-stopexecutioninput
source_filename: step-functions-stopexecutioninput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StopExecutionInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {},\n    \"error\": {},\n    \"cause\": {}\n  },\n  \"required\": [\n    \"executionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-stopexecutioninput-schema.json
tags:
- iPaaS
- Orchestration
- Serverless
title: StopExecutionInput
---
