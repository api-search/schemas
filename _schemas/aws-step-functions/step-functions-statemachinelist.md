---
description: ''
layout: schema
name: StateMachineList
properties_list: []
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-statemachinelist-schema.json
slug: step-functions-statemachinelist
source_filename: step-functions-statemachinelist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StateMachineList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"stateMachineArn\": {},\n      \"name\": {},\n      \"type\": {},\n      \"creationDate\": {}\n    },\n    \"required\": [\n      \"stateMachineArn\",\n      \"name\",\n      \"type\",\n      \"creationDate\"\n    ],\n    \"description\": \"Contains details about the state machine.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-statemachinelist-schema.json
tags:
- iPaaS
- Orchestration
- Serverless
title: StateMachineList
---
