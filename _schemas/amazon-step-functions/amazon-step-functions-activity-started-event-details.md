---
description: Contains details about the start of an activity during an execution.
layout: schema
name: ActivityStartedEventDetails
properties_list:
- description: ''
  name: workerName
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-activity-started-event-details-schema.json
slug: amazon-step-functions-activity-started-event-details
source_filename: amazon-step-functions-activity-started-event-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-activity-started-event-details-schema.json\",\n  \"title\": \"ActivityStartedEventDetails\",\n  \"description\": \"Contains details about the start of an activity during an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identity\"\n        },\n        {\n          \"description\": \"The name of the worker that the task is assigned to. These names are provided by the workers when calling <a>GetActivityTask</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-activity-started-event-details-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: ActivityStartedEventDetails
---
