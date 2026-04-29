---
description: Contains details about a Lambda function scheduled during an execution.
layout: schema
name: LambdaFunctionScheduledEventDetails
properties_list:
- description: ''
  name: resource
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: inputDetails
  type: object
- description: ''
  name: timeoutInSeconds
  type: object
- description: ''
  name: taskCredentials
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-lambdafunctionscheduledeventdetails-schema.json
slug: step-functions-lambdafunctionscheduledeventdetails
source_filename: step-functions-lambdafunctionscheduledeventdetails-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LambdaFunctionScheduledEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resource\": {},\n    \"input\": {},\n    \"inputDetails\": {},\n    \"timeoutInSeconds\": {},\n    \"taskCredentials\": {}\n  },\n  \"required\": [\n    \"resource\"\n  ],\n  \"description\": \"Contains details about a Lambda function scheduled during an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-lambdafunctionscheduledeventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: LambdaFunctionScheduledEventDetails
---
