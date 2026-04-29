---
description: An employer group record.
layout: schema
name: Group
properties_list:
- description: Unique employer group identifier.
  name: group_id
  type: string
- description: Employer group name.
  name: name
  type: string
- description: Legal employer name.
  name: employer_name
  type: string
- description: Group status.
  name: status
  type: string
- description: Number of enrolled employees.
  name: employee_count
  type: integer
- description: Group effective date.
  name: effective_date
  type: string
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-group-schema.json
slug: enterprise-connect-group
source_filename: enterprise-connect-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-group-schema.json\",\n  \"title\": \"Group\",\n  \"description\": \"An employer group record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique employer group identifier.\",\n      \"example\": \"GRP-123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Employer group name.\",\n      \"example\": \"Example Corp Benefits Group\"\n    },\n    \"employer_name\": {\n      \"type\": \"string\",\n      \"description\": \"Legal employer name.\",\n      \"example\": \"Example Corporation\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Group status.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ],\n      \"example\": \"active\"\
  \n    },\n    \"employee_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of enrolled employees.\",\n      \"example\": 250\n    },\n    \"effective_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Group effective date.\",\n      \"example\": \"2025-01-01\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-group-schema.json
tags: []
title: Group
---
