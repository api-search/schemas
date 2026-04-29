---
description: Contains details about a task scheduled during an execution.
layout: schema
name: TaskScheduledEventDetails
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resource
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: parameters
  type: object
- description: ''
  name: timeoutInSeconds
  type: object
- description: ''
  name: heartbeatInSeconds
  type: object
- description: ''
  name: taskCredentials
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-taskscheduledeventdetails-schema.json
slug: step-functions-taskscheduledeventdetails
source_filename: step-functions-taskscheduledeventdetails-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskScheduledEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {},\n    \"resource\": {},\n    \"region\": {},\n    \"parameters\": {},\n    \"timeoutInSeconds\": {},\n    \"heartbeatInSeconds\": {},\n    \"taskCredentials\": {}\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resource\",\n    \"region\",\n    \"parameters\"\n  ],\n  \"description\": \"Contains details about a task scheduled during an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-taskscheduledeventdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: TaskScheduledEventDetails
---
