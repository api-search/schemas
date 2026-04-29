---
description: Response containing matching pipeline object IDs.
layout: schema
name: Query Objects Output
properties_list:
- description: ''
  name: ids
  type: array
- description: ''
  name: hasMoreResults
  type: boolean
- description: ''
  name: marker
  type: string
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
schema_file: json-schema/query-objects-output-schema.json
slug: query-objects-output
source_filename: query-objects-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-pipeline/json-schema/query-objects-output-schema.json\",\n  \"title\": \"Query Objects Output\",\n  \"description\": \"Response containing matching pipeline object IDs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"hasMoreResults\": {\n      \"type\": \"boolean\"\n    },\n    \"marker\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/json-schema/query-objects-output-schema.json
tags:
- AWS
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
title: Query Objects Output
---
