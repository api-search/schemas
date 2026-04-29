---
description: Request to write values to a range.
layout: schema
name: RangeInput
properties_list:
- description: 2D array of values to write.
  name: values
  type: array
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-rangeinput-schema.json
slug: excel-api-rangeinput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RangeInput\",\n  \"description\": \"Request to write values to a range.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"2D array of values to write.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-rangeinput-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: RangeInput
---
