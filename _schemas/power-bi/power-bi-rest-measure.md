---
description: A DAX measure defined on a table
layout: schema
name: Measure
properties_list:
- description: The name of the measure
  name: name
  type: string
- description: The DAX expression for the measure
  name: expression
  type: string
- description: Optional format string
  name: formatString
  type: string
- description: Whether the measure is hidden in reports
  name: isHidden
  type: boolean
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-measure-schema.json
slug: power-bi-rest-measure
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Measure\",\n  \"type\": \"object\",\n  \"description\": \"A DAX measure defined on a table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the measure\"\n    },\n    \"expression\": {\n      \"type\": \"string\",\n      \"description\": \"The DAX expression for the measure\"\n    },\n    \"formatString\": {\n      \"type\": \"string\",\n      \"description\": \"Optional format string\"\n    },\n    \"isHidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the measure is hidden in reports\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-measure-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Measure
---
