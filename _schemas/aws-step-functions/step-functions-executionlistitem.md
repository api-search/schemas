---
description: Contains details about an execution.
layout: schema
name: ExecutionListItem
properties_list:
- description: ''
  name: executionArn
  type: object
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: startDate
  type: object
- description: ''
  name: stopDate
  type: object
- description: ''
  name: mapRunArn
  type: object
- description: ''
  name: itemCount
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-executionlistitem-schema.json
slug: step-functions-executionlistitem
source_filename: step-functions-executionlistitem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecutionListItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {},\n    \"stateMachineArn\": {},\n    \"name\": {},\n    \"status\": {},\n    \"startDate\": {},\n    \"stopDate\": {},\n    \"mapRunArn\": {},\n    \"itemCount\": {}\n  },\n  \"required\": [\n    \"executionArn\",\n    \"stateMachineArn\",\n    \"name\",\n    \"status\",\n    \"startDate\"\n  ],\n  \"description\": \"Contains details about an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-executionlistitem-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: ExecutionListItem
---
