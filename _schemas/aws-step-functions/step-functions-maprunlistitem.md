---
description: Contains details about a specific Map Run.
layout: schema
name: MapRunListItem
properties_list:
- description: ''
  name: executionArn
  type: object
- description: ''
  name: mapRunArn
  type: object
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: startDate
  type: object
- description: ''
  name: stopDate
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-maprunlistitem-schema.json
slug: step-functions-maprunlistitem
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MapRunListItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {},\n    \"mapRunArn\": {},\n    \"stateMachineArn\": {},\n    \"startDate\": {},\n    \"stopDate\": {}\n  },\n  \"required\": [\n    \"executionArn\",\n    \"mapRunArn\",\n    \"stateMachineArn\",\n    \"startDate\"\n  ],\n  \"description\": \"Contains details about a specific Map Run.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-maprunlistitem-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: MapRunListItem
---
