---
description: The <code>LoggingConfiguration</code> data type is used to set CloudWatch Logs options.
layout: schema
name: LoggingConfiguration
properties_list:
- description: ''
  name: level
  type: object
- description: ''
  name: includeExecutionData
  type: object
- description: ''
  name: destinations
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-logging-configuration-schema.json
slug: amazon-step-functions-logging-configuration
source_filename: amazon-step-functions-logging-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-logging-configuration-schema.json\",\n  \"title\": \"LoggingConfiguration\",\n  \"description\": \"The <code>LoggingConfiguration</code> data type is used to set CloudWatch Logs options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"level\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"Defines which category of execution history events are logged.\"\n        }\n      ]\n    },\n    \"includeExecutionData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncludeExecutionData\"\n        },\n        {\n          \"description\": \"Determines whether execution data is included in your log. When set to <code>false</code>, data is excluded.\"\n  \
  \      }\n      ]\n    },\n    \"destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogDestinationList\"\n        },\n        {\n          \"description\": \"An array of objects that describes where your execution history events will be logged. Limited to size 1. Required, if your log level is not set to <code>OFF</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-logging-configuration-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: LoggingConfiguration
---
