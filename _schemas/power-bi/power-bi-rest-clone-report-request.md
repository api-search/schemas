---
description: Request body for cloning a report
layout: schema
name: CloneReportRequest
properties_list:
- description: The name for the cloned report
  name: name
  type: string
- description: Optional dataset ID to rebind the cloned report to
  name: targetModelId
  type: string
- description: Optional workspace ID for the cloned report
  name: targetWorkspaceId
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-clone-report-request-schema.json
slug: power-bi-rest-clone-report-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CloneReportRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for cloning a report\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the cloned report\"\n    },\n    \"targetModelId\": {\n      \"type\": \"string\",\n      \"description\": \"Optional dataset ID to rebind the cloned report to\"\n    },\n    \"targetWorkspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"Optional workspace ID for the cloned report\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-clone-report-request-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: CloneReportRequest
---
