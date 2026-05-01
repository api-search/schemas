---
description: Provides details about input or output in an execution history event.
layout: schema
name: HistoryEventExecutionDataDetails
properties_list:
- description: ''
  name: truncated
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-history-event-execution-data-details-schema.json
slug: amazon-step-functions-history-event-execution-data-details
source_filename: amazon-step-functions-history-event-execution-data-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-history-event-execution-data-details-schema.json\",\n  \"title\": \"HistoryEventExecutionDataDetails\",\n  \"description\": \"Provides details about input or output in an execution history event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"truncated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/truncated\"\n        },\n        {\n          \"description\": \"Indicates whether input or output was truncated in the response. Always <code>false</code> for API calls.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-history-event-execution-data-details-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: HistoryEventExecutionDataDetails
---
