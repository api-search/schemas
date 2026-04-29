---
description: ''
layout: schema
name: MapRunList
properties_list: []
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-maprunlist-schema.json
slug: step-functions-maprunlist
source_filename: step-functions-maprunlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MapRunList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"executionArn\": {},\n      \"mapRunArn\": {},\n      \"stateMachineArn\": {},\n      \"startDate\": {},\n      \"stopDate\": {}\n    },\n    \"required\": [\n      \"executionArn\",\n      \"mapRunArn\",\n      \"stateMachineArn\",\n      \"startDate\"\n    ],\n    \"description\": \"Contains details about a specific Map Run.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-maprunlist-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: MapRunList
---
