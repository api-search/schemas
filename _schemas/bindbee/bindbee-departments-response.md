---
description: List of departments.
layout: schema
name: DepartmentsResponse
properties_list:
- description: Array of department records.
  name: data
  type: array
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-departments-response-schema.json
slug: bindbee-departments-response
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DepartmentsResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of departments.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of department records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Department\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-departments-response-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: DepartmentsResponse
---
