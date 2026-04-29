---
description: Selects whether or not the state machine's X-Ray tracing is enabled. Default is <code>false</code>
layout: schema
name: TracingConfiguration
properties_list:
- description: ''
  name: enabled
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-tracing-configuration-schema.json
slug: amazon-step-functions-tracing-configuration
source_filename: amazon-step-functions-tracing-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-tracing-configuration-schema.json\",\n  \"title\": \"TracingConfiguration\",\n  \"description\": \"Selects whether or not the state machine's X-Ray tracing is enabled. Default is <code>false</code> \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Enabled\"\n        },\n        {\n          \"description\": \"When set to <code>true</code>, X-Ray tracing is enabled.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-tracing-configuration-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: TracingConfiguration
---
