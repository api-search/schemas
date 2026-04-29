---
description: Contains details about the start of a task during an execution.
layout: schema
name: TaskStartedEventDetails
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resource
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-taskstartedeventdetails-schema.json
slug: step-functions-taskstartedeventdetails
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskStartedEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {},\n    \"resource\": {}\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resource\"\n  ],\n  \"description\": \"Contains details about the start of a task during an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-taskstartedeventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: TaskStartedEventDetails
---
