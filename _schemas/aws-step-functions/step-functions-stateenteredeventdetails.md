---
description: Contains details about a state entered during an execution.
layout: schema
name: StateEnteredEventDetails
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: inputDetails
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-stateenteredeventdetails-schema.json
slug: step-functions-stateenteredeventdetails
source_filename: step-functions-stateenteredeventdetails-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StateEnteredEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {},\n    \"input\": {},\n    \"inputDetails\": {}\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"description\": \"Contains details about a state entered during an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-stateenteredeventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: StateEnteredEventDetails
---
