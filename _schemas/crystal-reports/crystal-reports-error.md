---
description: Error response from the API
layout: schema
name: Error
properties_list:
- description: Numeric error code
  name: error_code
  type: integer
- description: Human-readable error message
  name: message
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-error-schema.json
slug: crystal-reports-error
source_filename: crystal-reports-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Error response from the API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error_code\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric error code\",\n      \"example\": 401\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"Authentication token is missing or expired\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-error-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: Error
---
