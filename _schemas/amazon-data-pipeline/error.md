---
description: Standard error response from the Data Pipeline API.
layout: schema
name: Error
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: code
  type: string
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/error-schema.json
slug: error
source_filename: error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Standard error response from the Data Pipeline API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/error-schema.json
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Error
---
