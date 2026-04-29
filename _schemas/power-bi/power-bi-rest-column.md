---
description: A column in a dataset table
layout: schema
name: Column
properties_list:
- description: The column name
  name: name
  type: string
- description: The data type of the column
  name: dataType
  type: string
- description: Optional format string for the column
  name: formatString
  type: string
- description: Name of the column to sort by
  name: sortByColumn
  type: string
- description: Whether the column is hidden in reports
  name: isHidden
  type: boolean
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-column-schema.json
slug: power-bi-rest-column
source_filename: power-bi-rest-column-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Column\",\n  \"type\": \"object\",\n  \"description\": \"A column in a dataset table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The column name\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the column\"\n    },\n    \"formatString\": {\n      \"type\": \"string\",\n      \"description\": \"Optional format string for the column\"\n    },\n    \"sortByColumn\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the column to sort by\"\n    },\n    \"isHidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the column is hidden in reports\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-column-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Column
---
