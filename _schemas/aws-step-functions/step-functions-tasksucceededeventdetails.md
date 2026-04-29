---
description: Contains details about the successful completion of a task state.
layout: schema
name: TaskSucceededEventDetails
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resource
  type: object
- description: ''
  name: output
  type: object
- description: ''
  name: outputDetails
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-tasksucceededeventdetails-schema.json
slug: step-functions-tasksucceededeventdetails
source_filename: step-functions-tasksucceededeventdetails-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskSucceededEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {},\n    \"resource\": {},\n    \"output\": {},\n    \"outputDetails\": {}\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resource\"\n  ],\n  \"description\": \"Contains details about the successful completion of a task state.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-tasksucceededeventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: TaskSucceededEventDetails
---
