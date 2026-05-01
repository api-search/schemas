---
description: Contains details about an activity scheduled during an execution.
layout: schema
name: ActivityScheduledEventDetails
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
  name: heartbeatInSeconds
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-activityscheduledeventdetails-schema.json
slug: step-functions-activityscheduledeventdetails
source_filename: step-functions-activityscheduledeventdetails-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActivityScheduledEventDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resource\": {},\n    \"input\": {},\n    \"inputDetails\": {},\n    \"timeoutInSeconds\": {},\n    \"heartbeatInSeconds\": {}\n  },\n  \"required\": [\n    \"resource\"\n  ],\n  \"description\": \"Contains details about an activity scheduled during an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-activityscheduledeventdetails-schema.json
tags:
- iPaaS
- Orchestration
- Serverless
title: ActivityScheduledEventDetails
---
