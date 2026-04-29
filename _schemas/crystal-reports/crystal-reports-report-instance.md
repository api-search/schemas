---
description: A transient report instance
layout: schema
name: ReportInstance
properties_list:
- description: Name of the report
  name: report_name
  type: string
- description: URI of the created instance resource
  name: resource
  type: string
- description: Unique identifier of the instance
  name: id
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-report-instance-schema.json
slug: crystal-reports-report-instance
source_filename: crystal-reports-report-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-report-instance-schema.json\",\n  \"title\": \"ReportInstance\",\n  \"description\": \"A transient report instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"report_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the report\",\n      \"example\": \"WorldSalesReport.rpt\"\n    },\n    \"resource\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the created instance resource\",\n      \"example\": \"/biprws/infostore/5765/rpt/instance/abc123\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the instance\",\n      \"example\": \"abc123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-report-instance-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: ReportInstance
---
