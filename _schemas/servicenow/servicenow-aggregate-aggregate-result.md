---
description: The aggregate statistics result. Structure varies based on the requested aggregate types and group-by fields.
layout: schema
name: AggregateResult
properties_list:
- description: Contains the computed aggregate values organized by field name and aggregate type.
  name: stats
  type: object
- description: When group-by fields are specified, contains an entry for each unique group with its aggregate values.
  name: group_by
  type: array
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-aggregate-aggregate-result-schema.json
slug: servicenow-aggregate-aggregate-result
source_filename: servicenow-aggregate-aggregate-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The aggregate statistics result. Structure varies based on the requested aggregate types and group-by fields.\",\n  \"properties\": {\n    \"stats\": {\n      \"type\": \"object\",\n      \"description\": \"Contains the computed aggregate values organized by field name and aggregate type.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"count\": {\n          \"type\": \"string\",\n          \"description\": \"The total count of records matching the query.\"\n        }\n      }\n    },\n    \"group_by\": {\n      \"type\": \"array\",\n      \"description\": \"When group-by fields are specified, contains an entry for each unique group with its aggregate values.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AggregateResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-aggregate-aggregate-result-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: AggregateResult
---
