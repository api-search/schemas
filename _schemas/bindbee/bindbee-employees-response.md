---
description: Paginated list of employee records.
layout: schema
name: EmployeesResponse
properties_list:
- description: Array of employee records.
  name: data
  type: array
- description: Cursor for next page.
  name: next_cursor
  type: string
- description: Whether more records exist.
  name: has_more
  type: boolean
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-employees-response-schema.json
slug: bindbee-employees-response
source_filename: bindbee-employees-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"EmployeesResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of employee records.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of employee records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Employee\"\n      }\n    },\n    \"next_cursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for next page.\",\n      \"example\": \"cursor-xyz\"\n    },\n    \"has_more\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether more records exist.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-employees-response-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: EmployeesResponse
---
