---
description: A parameter that can be set when running the report
layout: schema
name: ReportParameter
properties_list:
- description: Parameter name
  name: name
  type: string
- description: Data type of the parameter
  name: type
  type: string
- description: Prompt text shown to the user
  name: prompt
  type: string
- description: Whether the parameter is required
  name: required
  type: boolean
- description: Default value for the parameter
  name: default_value
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-report-parameter-schema.json
slug: crystal-reports-report-parameter
source_filename: crystal-reports-report-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-report-parameter-schema.json\",\n  \"title\": \"ReportParameter\",\n  \"description\": \"A parameter that can be set when running the report\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter name\",\n      \"example\": \"StartDate\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the parameter\",\n      \"example\": \"Date\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Prompt text shown to the user\",\n      \"example\": \"Enter the start date\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the parameter is required\",\n      \"example\": true\n    },\n    \"default_value\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"Default value for the parameter\",\n      \"example\": \"2023-01-01\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-report-parameter-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: ReportParameter
---
