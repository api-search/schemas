---
description: Summary information about a Crystal Report
layout: schema
name: ReportSummary
properties_list:
- description: Internal name of the report
  name: report_name
  type: string
- description: Display title of the report
  name: report_title
  type: string
- description: ''
  name: file_format_version
  type: object
- description: Author of the report
  name: author
  type: string
- description: Subject of the report
  name: subject
  type: string
- description: Keywords associated with the report
  name: keywords
  type: string
- description: Comments about the report
  name: comments
  type: string
- description: Last time the report data was refreshed
  name: last_data_refresh_date
  type: string
- description: URI for exporting the report
  name: export_uri
  type: string
- description: URI for the OData data service
  name: service_uri
  type: string
- description: URI for editing or managing the report
  name: edit_uri
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-report-summary-schema.json
slug: crystal-reports-report-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-report-summary-schema.json\",\n  \"title\": \"ReportSummary\",\n  \"description\": \"Summary information about a Crystal Report\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"report_name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the report\",\n      \"example\": \"WorldSalesReport.rpt\"\n    },\n    \"report_title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title of the report\",\n      \"example\": \"World Sales Report\"\n    },\n    \"file_format_version\": {\n      \"$ref\": \"#/components/schemas/FileFormatVersion\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Author of the report\",\n      \"example\": \"John Smith\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"Subject of the report\",\n      \"example\": \"Global Sales Data\"\n    },\n    \"keywords\": {\n      \"type\": \"string\",\n      \"description\": \"Keywords associated with the report\",\n      \"example\": \"sales, quarterly, revenue\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Comments about the report\",\n      \"example\": \"Updated for Q4 2023 data\"\n    },\n    \"last_data_refresh_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last time the report data was refreshed\",\n      \"example\": \"2023-12-15T14:30:00Z\"\n    },\n    \"export_uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI for exporting the report\",\n      \"example\": \"/biprws/infostore/5765/rpt/export\"\n    },\n    \"service_uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI for the OData data service\",\n      \"example\": \"/biprws/infostore/5765/rpt/data.svc\"\
  \n    },\n    \"edit_uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI for editing or managing the report\",\n      \"example\": \"/biprws/infostore/5765/rpt/instance\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-report-summary-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: ReportSummary
---
