---
description: ''
layout: schema
name: Datafiniti Search Request
properties_list:
- description: Datafiniti query expression filtering records.
  name: query
  type: string
- description: ''
  name: num_records
  type: integer
- description: ''
  name: download
  type: boolean
- description: ''
  name: format
  type: string
- description: ''
  name: view
  type: string
provider_name: Datafiniti
provider_slug: datafiniti
schema_file: json-schema/search-request.json
slug: search-request
source_filename: search-request.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datafiniti/main/json-schema/search-request.json\",\n  \"title\": \"Datafiniti Search Request\",\n  \"type\": \"object\",\n  \"required\": [\"query\"],\n  \"properties\": {\n    \"query\": {\"type\": \"string\", \"description\": \"Datafiniti query expression filtering records.\"},\n    \"num_records\": {\"type\": \"integer\", \"minimum\": 1},\n    \"download\": {\"type\": \"boolean\"},\n    \"format\": {\"type\": \"string\", \"enum\": [\"JSON\", \"CSV\"]},\n    \"view\": {\"type\": \"string\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datafiniti/refs/heads/main/json-schema/search-request.json
tags:
- Business Data
- Data Aggregation
- Data as a Service
- People Data
- Product Data
- Property Data
title: Datafiniti Search Request
---
