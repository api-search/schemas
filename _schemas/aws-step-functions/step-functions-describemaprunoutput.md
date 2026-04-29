---
description: ''
layout: schema
name: DescribeMapRunOutput
properties_list:
- description: ''
  name: mapRunArn
  type: object
- description: ''
  name: executionArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: startDate
  type: object
- description: ''
  name: stopDate
  type: object
- description: ''
  name: maxConcurrency
  type: object
- description: ''
  name: toleratedFailurePercentage
  type: object
- description: ''
  name: toleratedFailureCount
  type: object
- description: ''
  name: itemCounts
  type: object
- description: ''
  name: executionCounts
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-describemaprunoutput-schema.json
slug: step-functions-describemaprunoutput
source_filename: step-functions-describemaprunoutput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeMapRunOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mapRunArn\": {},\n    \"executionArn\": {},\n    \"status\": {},\n    \"startDate\": {},\n    \"stopDate\": {},\n    \"maxConcurrency\": {},\n    \"toleratedFailurePercentage\": {},\n    \"toleratedFailureCount\": {},\n    \"itemCounts\": {},\n    \"executionCounts\": {}\n  },\n  \"required\": [\n    \"mapRunArn\",\n    \"executionArn\",\n    \"status\",\n    \"startDate\",\n    \"maxConcurrency\",\n    \"toleratedFailurePercentage\",\n    \"toleratedFailureCount\",\n    \"itemCounts\",\n    \"executionCounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-describemaprunoutput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: DescribeMapRunOutput
---
