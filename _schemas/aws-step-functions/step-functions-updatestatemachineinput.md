---
description: ''
layout: schema
name: UpdateStateMachineInput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: definition
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: loggingConfiguration
  type: object
- description: ''
  name: tracingConfiguration
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-updatestatemachineinput-schema.json
slug: step-functions-updatestatemachineinput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateStateMachineInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {},\n    \"definition\": {},\n    \"roleArn\": {},\n    \"loggingConfiguration\": {},\n    \"tracingConfiguration\": {}\n  },\n  \"required\": [\n    \"stateMachineArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-updatestatemachineinput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: UpdateStateMachineInput
---
