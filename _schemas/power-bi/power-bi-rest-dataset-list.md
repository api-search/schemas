---
description: A list of Power BI datasets
layout: schema
name: DatasetList
properties_list:
- description: ''
  name: value
  type: array
- description: OData context URL
  name: '@odata.context'
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-dataset-list-schema.json
slug: power-bi-rest-dataset-list
source_filename: power-bi-rest-dataset-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatasetList\",\n  \"type\": \"object\",\n  \"description\": \"A list of Power BI datasets\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\"\n    },\n    \"@odata.context\": {\n      \"type\": \"string\",\n      \"description\": \"OData context URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-dataset-list-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: DatasetList
---
