---
description: Contains details about the execution timeout that occurred during the execution.
layout: schema
name: ExecutionTimedOutEventDetails
properties_list:
- description: ''
  name: error
  type: object
- description: ''
  name: cause
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-executiontimedouteventdetails-schema.json
slug: step-functions-executiontimedouteventdetails
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecutionTimedOutEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {},\n    \"cause\": {}\n  },\n  \"description\": \"Contains details about the execution timeout that occurred during the execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-executiontimedouteventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: ExecutionTimedOutEventDetails
---
