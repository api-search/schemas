---
description: Paginated list of data quality rules
layout: schema
name: DataQualityRuleList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
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
schema_file: json-schema/adoc-api-data-quality-rule-list-schema.json
slug: adoc-api-data-quality-rule-list
source_filename: adoc-api-data-quality-rule-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/data-quality-rule-list.json\",\n  \"title\": \"DataQualityRuleList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of data quality rules\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"data-quality-rule.json\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"page\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-data-quality-rule-list-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: DataQualityRuleList
---
