---
description: Request body for describing pipelines.
layout: schema
name: Describe Pipelines Request
properties_list:
- description: ''
  name: pipelineIds
  type: array
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/describe-pipelines-request-schema.json
slug: describe-pipelines-request
source_filename: describe-pipelines-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/describe-pipelines-request-schema.json\",\n  \"title\": \"Describe Pipelines Request\",\n  \"description\": \"Request body for describing pipelines.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"pipelineIds\"\n  ],\n  \"properties\": {\n    \"pipelineIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/describe-pipelines-request-schema.json
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Describe Pipelines Request
---
