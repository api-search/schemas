---
description: A running total field
layout: schema
name: RunningTotal
properties_list:
- description: Running total field name
  name: name
  type: string
- description: Field being totaled
  name: field
  type: string
- description: Aggregation operation
  name: operation
  type: string
- description: Condition that resets the running total
  name: reset_condition
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-running-total-schema.json
slug: crystal-reports-running-total
source_filename: crystal-reports-running-total-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-running-total-schema.json\",\n  \"title\": \"RunningTotal\",\n  \"description\": \"A running total field\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Running total field name\",\n      \"example\": \"RunningTotal_OrderAmount\"\n    },\n    \"field\": {\n      \"type\": \"string\",\n      \"description\": \"Field being totaled\",\n      \"example\": \"Order Amount\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"Aggregation operation\",\n      \"example\": \"Sum\"\n    },\n    \"reset_condition\": {\n      \"type\": \"string\",\n      \"description\": \"Condition that resets the running total\",\n      \"example\": \"OnGroupChange\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-running-total-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: RunningTotal
---
