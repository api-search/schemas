---
description: Contains details about a task that failed to submit during an execution.
layout: schema
name: TaskSubmitFailedEventDetails
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resource
  type: object
- description: ''
  name: error
  type: object
- description: ''
  name: cause
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-tasksubmitfailedeventdetails-schema.json
slug: step-functions-tasksubmitfailedeventdetails
source_filename: step-functions-tasksubmitfailedeventdetails-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskSubmitFailedEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {},\n    \"resource\": {},\n    \"error\": {},\n    \"cause\": {}\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resource\"\n  ],\n  \"description\": \"Contains details about a task that failed to submit during an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-tasksubmitfailedeventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: TaskSubmitFailedEventDetails
---
