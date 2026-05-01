---
description: UpdateMapRunInput schema from Amazon Step Functions API
layout: schema
name: UpdateMapRunInput
properties_list:
- description: ''
  name: mapRunArn
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
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-update-map-run-input-schema.json
slug: amazon-step-functions-update-map-run-input
source_filename: amazon-step-functions-update-map-run-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-map-run-input-schema.json\",\n  \"title\": \"UpdateMapRunInput\",\n  \"description\": \"UpdateMapRunInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mapRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a Map Run.\"\n        }\n      ]\n    },\n    \"maxConcurrency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxConcurrency\"\n        },\n        {\n          \"description\": \"The maximum number of child workflow executions that can be specified to run in parallel for the Map Run at the same time.\"\n        }\n      ]\n    },\n    \"toleratedFailurePercentage\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ToleratedFailurePercentage\"\n        },\n        {\n          \"description\": \"The maximum percentage of failed items before the Map Run fails.\"\n        }\n      ]\n    },\n    \"toleratedFailureCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ToleratedFailureCount\"\n        },\n        {\n          \"description\": \"The maximum number of failed items before the Map Run fails.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"mapRunArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-update-map-run-input-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: UpdateMapRunInput
---
