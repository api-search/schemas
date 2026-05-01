---
description: Request body for activating a pipeline.
layout: schema
name: Activate Pipeline Request
properties_list:
- description: ''
  name: pipelineId
  type: string
- description: ''
  name: startTimestamp
  type: string
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/activate-pipeline-request-schema.json
slug: activate-pipeline-request
source_filename: activate-pipeline-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/activate-pipeline-request-schema.json\",\n  \"title\": \"Activate Pipeline Request\",\n  \"description\": \"Request body for activating a pipeline.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"pipelineId\"\n  ],\n  \"properties\": {\n    \"pipelineId\": {\n      \"type\": \"string\"\n    },\n    \"startTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/activate-pipeline-request-schema.json
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Activate Pipeline Request
---
