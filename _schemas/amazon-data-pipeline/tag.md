---
description: A key-value tag pair applied to a pipeline resource.
layout: schema
name: Tag
properties_list:
- description: The tag key
  name: key
  type: string
- description: The tag value
  name: value
  type: string
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/tag-schema.json
slug: tag
source_filename: tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A key-value tag pair applied to a pipeline resource.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"key\",\n    \"value\"\n  ],\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The tag key\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The tag value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/tag-schema.json
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Tag
---
