---
description: Contains details about a Map Run that was started during a state machine execution.
layout: schema
name: MapRunStartedEventDetails
properties_list:
- description: ''
  name: mapRunArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-map-run-started-event-details-schema.json
slug: amazon-step-functions-map-run-started-event-details
source_filename: amazon-step-functions-map-run-started-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-run-started-event-details-schema.json\",\n  \"title\": \"MapRunStartedEventDetails\",\n  \"description\": \"Contains details about a Map Run that was started during a state machine execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mapRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a Map Run that was started.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-run-started-event-details-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: MapRunStartedEventDetails
---
