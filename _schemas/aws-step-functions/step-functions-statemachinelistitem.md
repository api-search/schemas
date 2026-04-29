---
description: Contains details about the state machine.
layout: schema
name: StateMachineListItem
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: creationDate
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-statemachinelistitem-schema.json
slug: step-functions-statemachinelistitem
source_filename: step-functions-statemachinelistitem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StateMachineListItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {},\n    \"name\": {},\n    \"type\": {},\n    \"creationDate\": {}\n  },\n  \"required\": [\n    \"stateMachineArn\",\n    \"name\",\n    \"type\",\n    \"creationDate\"\n  ],\n  \"description\": \"Contains details about the state machine.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-statemachinelistitem-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: StateMachineListItem
---
