---
description: ''
layout: schema
name: CreateStateMachineInput
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: definition
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: loggingConfiguration
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: tracingConfiguration
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-createstatemachineinput-schema.json
slug: step-functions-createstatemachineinput
source_filename: step-functions-createstatemachineinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateStateMachineInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {},\n    \"definition\": {},\n    \"roleArn\": {},\n    \"type\": {},\n    \"loggingConfiguration\": {},\n    \"tags\": {},\n    \"tracingConfiguration\": {}\n  },\n  \"required\": [\n    \"name\",\n    \"definition\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-createstatemachineinput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: CreateStateMachineInput
---
