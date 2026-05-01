---
description: A key-value pair defining a pipeline object property.
layout: schema
name: Field
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: stringValue
  type: string
- description: ''
  name: refValue
  type: string
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/field-schema.json
slug: field
source_filename: field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/field-schema.json\",\n  \"title\": \"Field\",\n  \"description\": \"A key-value pair defining a pipeline object property.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"key\"\n  ],\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"stringValue\": {\n      \"type\": \"string\"\n    },\n    \"refValue\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/field-schema.json
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Field
---
