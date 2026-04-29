---
description: Provides details about execution input or output.
layout: schema
name: CloudWatchEventsExecutionDataDetails
properties_list:
- description: ''
  name: included
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-cloud-watch-events-execution-data-details-schema.json
slug: amazon-step-functions-cloud-watch-events-execution-data-details
source_filename: amazon-step-functions-cloud-watch-events-execution-data-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-cloud-watch-events-execution-data-details-schema.json\",\n  \"title\": \"CloudWatchEventsExecutionDataDetails\",\n  \"description\": \"Provides details about execution input or output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"included\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/includedDetails\"\n        },\n        {\n          \"description\": \"Indicates whether input or output was included in the response. Always <code>true</code> for API calls. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-cloud-watch-events-execution-data-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: CloudWatchEventsExecutionDataDetails
---
