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
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-loggingconfiguration-schema.json
slug: step-functions-loggingconfiguration
source_filename: step-functions-loggingconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoggingConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"level\": {},\n    \"includeExecutionData\": {},\n    \"destinations\": {}\n  },\n  \"description\": \"The <code>LoggingConfiguration</code> data type is used to set CloudWatch Logs options.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-loggingconfiguration-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: LoggingConfiguration
---
