---
description: Contains details about a specific Map Run.
layout: schema
name: MapRunListItem
properties_list:
- description: ''
  name: executionArn
  type: object
- description: ''
  name: mapRunArn
  type: object
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: startDate
  type: object
- description: ''
  name: stopDate
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-map-run-list-item-schema.json
slug: amazon-step-functions-map-run-list-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-run-list-item-schema.json\",\n  \"title\": \"MapRunListItem\",\n  \"description\": \"Contains details about a specific Map Run.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The <code>executionArn</code> of the execution from which the Map Run was started.\"\n        }\n      ]\n    },\n    \"mapRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Map Run.\"\n        }\n      ]\n    },\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the executed state machine.\"\n        }\n      ]\n    },\n    \"startDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date on which the Map Run started.\"\n        }\n      ]\n    },\n    \"stopDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date on which the Map Run stopped.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"executionArn\",\n    \"mapRunArn\",\n    \"stateMachineArn\",\n    \"startDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-run-list-item-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: MapRunListItem
---
