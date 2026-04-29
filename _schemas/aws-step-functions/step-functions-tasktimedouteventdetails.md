---
description: Contains details about a resource timeout that occurred during an execution.
layout: schema
name: TaskTimedOutEventDetails
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
schema_file: json-schema/step-functions-tasktimedouteventdetails-schema.json
slug: step-functions-tasktimedouteventdetails
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskTimedOutEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {},\n    \"resource\": {},\n    \"error\": {},\n    \"cause\": {}\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resource\"\n  ],\n  \"description\": \"Contains details about a resource timeout that occurred during an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-tasktimedouteventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: TaskTimedOutEventDetails
---
