---
description: Paginated list of alerts
layout: schema
name: AlertList
properties_list:
- description: ''
  name: data
  type: array
- description: Total alert count
  name: total
  type: integer
- description: ''
  name: page
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-alert-list-schema.json
slug: adoc-api-alert-list
source_filename: adoc-api-alert-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/alert-list.json\",\n  \"title\": \"AlertList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of alerts\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"alert.json\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total alert count\"\n    },\n    \"page\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-alert-list-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: AlertList
---
