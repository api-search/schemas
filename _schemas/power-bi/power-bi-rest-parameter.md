---
description: A parameter in a dataset
layout: schema
name: Parameter
properties_list:
- description: The parameter name
  name: name
  type: string
- description: The data type of the parameter
  name: type
  type: string
- description: The current value of the parameter
  name: currentValue
  type: string
- description: Whether the parameter is required
  name: isRequired
  type: boolean
- description: Suggested values for the parameter
  name: suggestedValues
  type: array
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-parameter-schema.json
slug: power-bi-rest-parameter
source_filename: power-bi-rest-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Parameter\",\n  \"type\": \"object\",\n  \"description\": \"A parameter in a dataset\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The parameter name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the parameter\"\n    },\n    \"currentValue\": {\n      \"type\": \"string\",\n      \"description\": \"The current value of the parameter\"\n    },\n    \"isRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the parameter is required\"\n    },\n    \"suggestedValues\": {\n      \"type\": \"array\",\n      \"description\": \"Suggested values for the parameter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-parameter-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Parameter
---
