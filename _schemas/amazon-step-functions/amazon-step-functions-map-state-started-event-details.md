---
description: Details about a Map state that was started.
layout: schema
name: MapStateStartedEventDetails
properties_list:
- description: ''
  name: length
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-map-state-started-event-details-schema.json
slug: amazon-step-functions-map-state-started-event-details
source_filename: amazon-step-functions-map-state-started-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-state-started-event-details-schema.json\",\n  \"title\": \"MapStateStartedEventDetails\",\n  \"description\": \"Details about a Map state that was started.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"length\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnsignedInteger\"\n        },\n        {\n          \"description\": \"The size of the array for Map state iterations.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-map-state-started-event-details-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: MapStateStartedEventDetails
---
