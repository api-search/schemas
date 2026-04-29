---
description: The report response containing an array of report entries. Column names correspond to the report field definitions.
layout: schema
name: ReportResponse
properties_list:
- description: The array of report data rows.
  name: Report_Entry
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/raas-report-response-schema.json
slug: raas-report-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportResponse\",\n  \"type\": \"object\",\n  \"description\": \"The report response containing an array of report entries. Column names correspond to the report field definitions.\",\n  \"properties\": {\n    \"Report_Entry\": {\n      \"type\": \"array\",\n      \"description\": \"The array of report data rows.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/raas-report-response-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: ReportResponse
---
