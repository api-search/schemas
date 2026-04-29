---
description: Contains details about a lambda function that failed to start during an execution.
layout: schema
name: LambdaFunctionStartFailedEventDetails
properties_list:
- description: ''
  name: error
  type: object
- description: ''
  name: cause
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-lambdafunctionstartfailedeventdetails-schema.json
slug: step-functions-lambdafunctionstartfailedeventdetails
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LambdaFunctionStartFailedEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {},\n    \"cause\": {}\n  },\n  \"description\": \"Contains details about a lambda function that failed to start during an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-lambdafunctionstartfailedeventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: LambdaFunctionStartFailedEventDetails
---
