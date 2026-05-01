---
description: Request body for creating a new pipeline.
layout: schema
name: Create Pipeline Request
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: uniqueId
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: tags
  type: array
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/create-pipeline-request-schema.json
slug: create-pipeline-request
source_filename: create-pipeline-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/create-pipeline-request-schema.json\",\n  \"title\": \"Create Pipeline Request\",\n  \"description\": \"Request body for creating a new pipeline.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"uniqueId\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"uniqueId\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/create-pipeline-request-schema.json
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Create Pipeline Request
---
