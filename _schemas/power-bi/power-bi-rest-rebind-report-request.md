---
description: Request body for rebinding a report to a different dataset
layout: schema
name: RebindReportRequest
properties_list:
- description: The ID of the target dataset
  name: datasetId
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-rebind-report-request-schema.json
slug: power-bi-rest-rebind-report-request
source_filename: power-bi-rest-rebind-report-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RebindReportRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for rebinding a report to a different dataset\",\n  \"properties\": {\n    \"datasetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the target dataset\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-rebind-report-request-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: RebindReportRequest
---
