---
description: Microsoft Graph API error response.
layout: schema
name: ErrorResponse
properties_list:
- description: Error details.
  name: error
  type: object
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-errorresponse-schema.json
slug: excel-api-errorresponse
source_filename: excel-api-errorresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Microsoft Graph API error response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Error details.\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Error code.\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Error message.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-errorresponse-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: ErrorResponse
---
