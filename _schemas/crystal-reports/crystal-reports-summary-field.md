---
description: A summary or aggregate field in the report
layout: schema
name: SummaryField
properties_list:
- description: Summary field name
  name: name
  type: string
- description: Aggregation operation
  name: operation
  type: string
- description: Source field being summarized
  name: field
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-summary-field-schema.json
slug: crystal-reports-summary-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-summary-field-schema.json\",\n  \"title\": \"SummaryField\",\n  \"description\": \"A summary or aggregate field in the report\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Summary field name\",\n      \"example\": \"Sum of Order Amount\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"Aggregation operation\",\n      \"example\": \"Sum\"\n    },\n    \"field\": {\n      \"type\": \"string\",\n      \"description\": \"Source field being summarized\",\n      \"example\": \"Order Amount\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-summary-field-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: SummaryField
---
