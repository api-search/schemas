---
description: An error found during pipeline definition validation.
layout: schema
name: Validation Error
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: errors
  type: array
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/validation-error-schema.json
slug: validation-error
source_filename: validation-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/validation-error-schema.json\",\n  \"title\": \"Validation Error\",\n  \"description\": \"An error found during pipeline definition validation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/validation-error-schema.json
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Validation Error
---
