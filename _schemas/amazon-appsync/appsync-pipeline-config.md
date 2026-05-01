---
description: Pipeline resolver configuration
layout: schema
name: PipelineConfig
properties_list:
- description: List of function IDs in the pipeline
  name: functions
  type: array
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-pipeline-config-schema.json
slug: appsync-pipeline-config
source_filename: appsync-pipeline-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-pipeline-config-schema.json\",\n  \"title\": \"PipelineConfig\",\n  \"description\": \"Pipeline resolver configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functions\": {\n      \"type\": \"array\",\n      \"description\": \"List of function IDs in the pipeline\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-pipeline-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: PipelineConfig
---
