---
description: ''
layout: schema
name: ExecutionList
properties_list: []
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-executionlist-schema.json
slug: step-functions-executionlist
source_filename: step-functions-executionlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecutionList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"executionArn\": {},\n      \"stateMachineArn\": {},\n      \"name\": {},\n      \"status\": {},\n      \"startDate\": {},\n      \"stopDate\": {},\n      \"mapRunArn\": {},\n      \"itemCount\": {}\n    },\n    \"required\": [\n      \"executionArn\",\n      \"stateMachineArn\",\n      \"name\",\n      \"status\",\n      \"startDate\"\n    ],\n    \"description\": \"Contains details about an execution.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-executionlist-schema.json
tags:
- iPaaS
- Orchestration
- Serverless
title: ExecutionList
---
