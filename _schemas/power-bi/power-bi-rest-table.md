---
description: A table within a Power BI dataset
layout: schema
name: Table
properties_list:
- description: The name of the table
  name: name
  type: string
- description: The columns in the table
  name: columns
  type: array
- description: Rows of data in the table
  name: rows
  type: array
- description: DAX measures defined on the table
  name: measures
  type: array
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-table-schema.json
slug: power-bi-rest-table
source_filename: power-bi-rest-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Table\",\n  \"type\": \"object\",\n  \"description\": \"A table within a Power BI dataset\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"The columns in the table\"\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"description\": \"Rows of data in the table\"\n    },\n    \"measures\": {\n      \"type\": \"array\",\n      \"description\": \"DAX measures defined on the table\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-table-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Table
---
