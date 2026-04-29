---
description: Paginated list of enrollment records.
layout: schema
name: EnrollmentList
properties_list:
- description: Array of enrollment records.
  name: items
  type: array
- description: Total number of matching enrollments.
  name: total
  type: integer
- description: Maximum number of results returned.
  name: limit
  type: integer
- description: Number of results skipped.
  name: offset
  type: integer
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-enrollment-list-schema.json
slug: enterprise-connect-enrollment-list
source_filename: enterprise-connect-enrollment-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-enrollment-list-schema.json\",\n  \"title\": \"EnrollmentList\",\n  \"description\": \"Paginated list of enrollment records.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Array of enrollment records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Enrollment\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching enrollments.\",\n      \"example\": 150\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results returned.\",\n      \"example\": 50\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of\
  \ results skipped.\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-enrollment-list-schema.json
tags: []
title: EnrollmentList
---
