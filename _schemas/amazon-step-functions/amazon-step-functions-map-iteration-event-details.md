---
description: Contains details about an iteration of a Map state.
layout: schema
name: MapIterationEventDetails
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: index
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-map-iteration-event-details-schema.json
slug: amazon-step-functions-map-iteration-event-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-iteration-event-details-schema.json\",\n  \"title\": \"MapIterationEventDetails\",\n  \"description\": \"Contains details about an iteration of a Map state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the iteration\\u2019s parent Map state.\"\n        }\n      ]\n    },\n    \"index\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedInteger\"\n        },\n        {\n          \"description\": \"The index of the array belonging to the Map state iteration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-iteration-event-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: MapIterationEventDetails
---
