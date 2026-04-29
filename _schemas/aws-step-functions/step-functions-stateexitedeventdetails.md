---
description: Contains details about an exit from a state during an execution.
layout: schema
name: StateExitedEventDetails
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: output
  type: object
- description: ''
  name: outputDetails
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-stateexitedeventdetails-schema.json
slug: step-functions-stateexitedeventdetails
source_filename: step-functions-stateexitedeventdetails-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StateExitedEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {},\n    \"output\": {},\n    \"outputDetails\": {}\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"description\": \"Contains details about an exit from a state during an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-stateexitedeventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: StateExitedEventDetails
---
